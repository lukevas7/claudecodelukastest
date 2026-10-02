---
description: Build a Gearline Cycles page from a brief, then critique, fix, polish, audit, commit, push to main and preview it, without stopping for approval
argument-hint: <page brief>
---

# /page: build, review and ship a Gearline page

Brief: $ARGUMENTS

The user has pre-approved this whole run. Do not ask questions and do not stop for approval at any step, including steps where a skill or reference would normally ask (critique's closing questions, new-work's direction or concept round, comp approval, build-path offers). Where a step would ask, apply the standing answers below, print one line saying which default you applied, and continue.

If the brief is empty, stop and say that `/page` needs a brief, for example `/page product detail page for the Trailblazer G2 Gravel`.

## Standing answers

- **Design system:** `bike-shop/DESIGN.md` and its sidecar `bike-shop/.impeccable/design.json` are law. Never change their colours, fonts, type scale, radii, shadows or component styles, and never edit either file during this command. If a finding seems to need a new colour, font or style, solve it inside the system or leave it and list it as "needs a design-system decision" in the summary.
- **Product truth:** `bike-shop/PRODUCT.md`. All content is fictional demo material. Reuse the brands, prices, policies and the 4.8/5 from 2,300 reviews rating it names. Do not invent testimonials, customer names, press quotes, awards or statistics. Missing product facts become clearly labelled placeholders such as `[PRICE]`.
- **Scope of fixes:** fix every P0 and P1 issue that critique and audit report. P2 and P3 only when the fix is a one-line change inside the system; list the rest.
- **Build path:** code-first. No image generation, no comps, no concept-seed roll, no decision page. The brief, PRODUCT.md and DESIGN.md decide the structure.
- **Images:** no external images. Use labelled placeholders in DESIGN.md's flat placeholder style, for example "Product photo: gravel bike, side view".
- **Out of bounds:** `dashboard.html`, `figma-export/` and the other `bike-shop/hero-*.html` directions. Do not read them for style and do not edit them.

## 1. Load context

1. Read `bike-shop/PRODUCT.md` and `bike-shop/DESIGN.md` in full, and skim the components in `bike-shop/.impeccable/design.json`.
2. Choose a short kebab-case page name from the brief (for example `product-trailblazer-g2`, `deals`, `bike-finder`). If `bike-shop/<page-name>.html` already exists, rebuild it in place and say so.
3. Run `.claude/skills/impeccable/scripts/impeccable context --target bike-shop/<page-name>.html` once and follow its directives, within the standing answers above.

## 2. Build the page

Use the impeccable skill for the build: invoke it with the brief, target `bike-shop/<page-name>.html`, and the standing answers. It loads `reference/new-work.md` (a whole surface inside an established world) and `reference/craft-floor.md`. Within that flow:

- Pick the visitor mode from the surface (a shop page is usually Persuade; a comparison table or account page is Operate) and the structure that serves PRODUCT.md's principles: clear prices, visible trust points, short path to cart.
- Write one self-contained static HTML file at `bike-shop/<page-name>.html`, matching the conventions of `bike-shop/hero-b.html`: the DESIGN.md tokens as CSS custom properties on `:root`, Archivo from Google Fonts, an inline SVG icon sprite, semantic landmarks, real `<button>` and `<a href>` elements, and responsive rules down to 390px wide.
- Every product shows current price, old price and discount when discounted, one key spec, stock status (dot plus words) and Add to cart. The trust points stay visible near the first decision.

**Parallel sections.** When the page has four or more independent sections, build them in parallel:

1. Write the page shell first: `<head>`, the `:root` tokens, the base styles, the icon sprite, the header and an empty slot per section.
2. Spawn one subagent per independent section, all in the same message. Give each the brief, its section's job, the section's place in the reading order, and the paths of PRODUCT.md, DESIGN.md and the shell. Each returns its section markup plus CSS scoped under one section class, using only the shell's tokens and no new colours, fonts, radii or shadows. Each writes its result to the scratchpad directory, not into the page.
3. Merge the sections into the page yourself, remove duplicate rules, and check that spacing between sections follows one rhythm.

Fewer than four sections: build in one pass, no subagents.

Inspect once at desktop 1440×900 and mobile 390×844 with a headless browser. Confirm the fonts loaded before judging, because a fallback face changes every line break. Fix what the screenshots show in one batch.

## 3. Critique, then fix P0 and P1

Run `/impeccable critique bike-shop/<page-name>.html` through the impeccable skill. Run its assessments as subagents as the reference requires, persist the snapshot, and end the report with the line `Questions skipped: /page run, user pre-authorized fixing every P0 and P1 inside DESIGN.md` instead of asking. Then fix every P0 and P1 finding in one batch.

## 4. Polish

Run `/impeccable polish bike-shop/<page-name>.html`. It picks up the critique snapshot. Apply its fixes within the standing answers.

## 5. Audit, then fix remaining P0 and P1

Run `/impeccable audit bike-shop/<page-name>.html`. Fix every remaining P0 and P1 in one batch, then run `.claude/skills/impeccable/scripts/impeccable detect --json bike-shop/<page-name>.html` once and clear anything mechanical. For a finding that is a confirmed false positive, add the narrowest ignore with `impeccable hooks ignore-value` and a reason that names the evidence. Then take one final desktop and mobile screenshot round. Two inspection rounds after the build is the ceiling: stop polishing after that.

## 6. Ship

1. Stage only this page and anything this run created for it, such as `.impeccable/critique/` snapshots or a detector ignore. Never stage changes to DESIGN.md, the sidecar or the other hero directions.
2. Commit with a message naming the page, then `git push origin HEAD:main`. On a network failure, retry up to four times with backoff of 2s, 4s, 8s and 16s. If the push is rejected because main moved, fetch, rebase this commit onto `origin/main`, and push again. Never force-push.
3. Show the page in the preview: send `bike-shop/<page-name>.html` to the user rendered (SendUserFile with `display: render` where it exists, otherwise the harness's preview or open tool), plus the final desktop and mobile screenshots.

## 7. Summary

End with a short summary in plain language, no more than about 12 lines:

- **Built:** the page name and path, its sections in order, and the commit hash pushed to main.
- **Top fixes:** the three to five most important fixes from critique, polish and audit, each in one line with its severity.
- **Left open:** remaining P2 and P3 items, any "needs a design-system decision" items, and placeholders the user must replace with real content.
