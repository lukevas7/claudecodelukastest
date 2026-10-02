# Critique: bike-shop/hero-b.html (Direction B, "The Start List")

Method: dual-agent (A: a112d1d5ff2366325 · B: a7ec336b2444ef4f0)
Target state: `steps/00-original.html`. Mode: Persuade (shop homepage, hero plus Hot deals).

## Design Health Score

| # | Heuristic | Score | Key issue |
|---|---|---|---|
| 1 | Visibility of system status | 2 | Add to cart gives no feedback; the cart shows no count. |
| 2 | Match system / real world | 3 | Plain words and exact numbers, but "−17%" alone, no saving in euros. |
| 3 | User control and freedom | 2 | Product names are not links; the category nav vanishes under 900px with no replacement. |
| 4 | Consistency and standards | 3 | Identical card fields; the whole card lifts on hover although only the button is clickable. |
| 5 | Error prevention | 1 | Add to cart sits next to "Sizes S to XL" with no way to choose a size; no sold-out states. |
| 6 | Recognition rather than recall | 3 | Category, spec and stock all visible. |
| 7 | Flexibility and efficiency | n/a | Persuade surface. |
| 8 | Aesthetic and minimalist design | 3 | Strong, but 16 pin dots, a dashed tear line and an empty 200px photo block on mobile add noise. |
| 9 | Error recovery | 2 | No empty, failure or sold-out states designed. |
| 10 | Help and documentation | n/a | Persuade surface. |
| **Total** | | **19/32** | Acceptable, with clear P1 gaps. |

## Design specificity verdict

**Review:** Authored for this product. The race-programme idea (deal cards as race bibs), 62% condensed italic type, cobalt and yellow owning whole regions, and copy built on the real promise ("Ready in 48 hours") could not be swapped onto another shop unchanged. The generic parts are the trust icons and the paired hero buttons. The bib decoration (pin dots, dashed tear line) is where the concept tips into ornament.

**Deterministic scan:** CLI `impeccable detect`: 0 findings with project config. One `cramped-padding` finding on the trust strip appears with `--no-config`; it is the known false positive (the strip is inset by `clamp()` padding the static scan cannot resolve) and is already ignored with a reason. The in-page detector (live server on port 8400, injection succeeded) reported `oversized-h1` at 1440 (118px, 45vh); intentional display type for this Persuade hero, and the trust bar still lands at y 764 of 900. Nothing at 375. No horizontal overflow at either width. All measured text contrast pairs pass AA (lowest: nav links 6.42:1 on cobalt).

## Overall impression

The hero lands the promise in about two seconds and the yellow trust strip reassures. The deals section is where energy turns into friction: the eye reads a black "−17%" before the price, and "Add to cart" asks for a purchase without a size. The single biggest opportunity: make each card answer "what does it cost, what do I save, can I get my size" in that order.

## What's working

- The headline is the value proposition, with "Ready in 48 hours" in yellow, and the primary CTA sits inside the first viewport on desktop (y 640 to 708) and mobile.
- One straight trust band directly under the decision, not a badge cloud.
- Disciplined cards: identical field order, tabular figures, stock as dot plus words.

## Priority issues

1. **[P1] Price is not the strongest element on the card.** Discount 58px black, price 42px cobalt, old price 16px. Fix: price becomes the largest figure (about 56 to 60px cobalt); discount becomes a tag with the saving in euros; old price larger and tabular.
2. **[P1] Add to cart ignores sizes; no sold-out handling.** Fix: size chips on the card (44px targets, sold-out sizes struck and labelled), button labelled with the product, sold-out card state.
3. **[P1] Mobile has no navigation.** `.nav ul{display:none}` under 900px with no replacement. Fix: a scrollable category row under the header.
4. **[P1] Screen-reader names lost or ambiguous.** `aria-label` on plain `span` and `s` is often ignored, so the price reads "€1,899 €2,299"; four identical "Add to cart" names; logo reads "GearlineCycles". Fix: visually hidden text ("Now", "Was", "17% off"), product name in each button's accessible name, a real space in the logo.
5. **[P2] Mobile first viewport and decorative noise.** At 375×812 the trust strip runs to y 844, so its last item is below the fold; an empty 200px photo block sits before the deals; 4 pin dots and a dashed rule on every card; card hover tilts as if clickable. Fix: trust strip 2×2 on phones, drop the empty photo block on phones, remove pin dots, lift without tilt.

## Persona red flags

- **Deal hunter on mobile:** scrolls past the trust strip and an empty block before any deal; no euro saving; no category nav.
- **Unsure first-time buyer:** no size help; cannot open a product; "Find my bike" is quieter than it needs to be.
- **Screen-reader user:** ambiguous prices, four identical buttons, "GearlineCycles".

## Minor observations

- Category label 13px and plate caption 12.5px are small; raise to 14px and 13px or more.
- "5 left in stock" is red like "3 left"; keep red for 3 or fewer so red keeps its meaning.
- `.add` is not pinned to the card bottom; a two-line product name would misalign prices and buttons across the row.
- `.price s` turns tabular figures off.
- "Shop bikes" is generic; say what you shop.
- No `prefers-reduced-motion` guard on the hover lift and tilt.
- Cart link has no count.
- Nav links have a 16px-tall hit area (desktop only).
- Rating "4.8/5 2,300 reviews" reads as two unrelated numbers; "from" and a link to reviews would help.

## Questions

Questions skipped: unattended full pass, the user pre-authorized every step and asked these findings to guide layout, typeset, clarify, distill, quieter, harden, adapt, animate, polish and audit.
