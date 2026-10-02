---
target: bike-shop/hero-b.html
total_score: 19
max_score: 32
na_heuristics: 7,10
p0_count: 0
p1_count: 4
target_identity: "file:/home/user/claudecodelukastest/bike-shop/hero-b.html"
target_fingerprint: "sha256:35fc112fe4e3d649999d3e1b1ceed9f3c2156da25645477f1f3b7e78b06a6787"
target_path: /home/user/claudecodelukastest/bike-shop/hero-b.html
timestamp: 2026-10-02T06-00-10Z
slug: bike-shop-hero-b-html
---
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
