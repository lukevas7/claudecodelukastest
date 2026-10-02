# Full Impeccable pass on bike-shop/hero-b.html

Starting point: `00-original.html`. Every step edits the same file and saves a snapshot. Identity kept throughout: cobalt and yellow, condensed italic headlines, race-bib cards.

## 1. Critique (`critique.md`)
- Two independent assessments (design review and detector plus browser evidence). Score 19/32, 0 P0, 4 P1.
- P1s: price weaker than the discount, Add to cart with no size choice, no navigation on phones, screen-reader names lost or ambiguous.
- P2: at 375×812 the last trust point falls below the fold, an empty photo block sits before the deals on phones, and the pin dots add noise.

## 2. Layout (`01-layout.html`)
- Cards now read photo first, then category, name, price, spec and stock, with the button pinned to the bottom so prices and buttons line up across a row whatever the name length.
- On phones the trust strip is a 2×2 grid: it now ends at y 756 instead of 844 on a 375×812 screen, so all four points are above the fold.
- The hero itself was already balanced in the earlier layout pass (headline, line, Shop bikes in one column, CTA at y 640 to 708 at 1440×900), so it is unchanged.

## 3. Typeset (`02-typeset.html`)
- The current price is now the largest figure on each card (58px narrow cobalt, up from 42px), so the eye reads what the bike costs first.
- The discount moved from a 58px black number to a compact slanted tag (24px yellow on Tarmac), still the bib's number but no longer louder than the price.
- Small text raised: category label 13 to 14px, photo caption 12.5 to 13px, spec and stock row 14 to 15px, old price 16 to 18px with tabular figures restored.

## 4. Clarify (`03-clarify.html`)
- Each price now says what you save ("Was €2,299 · Save €400"), and screen readers hear "Now €1,899, Was €2,299, 17% off" through visually hidden text instead of ignored `aria-label`s.
- CTA and trust wording: "Shop bikes" became "Shop all bikes", "Free delivery over €500" became "Free delivery on orders over €500", and the rating reads "4.8/5 from 2,300 reviews" as one link. Each Add to cart button now names its bike for screen readers.
- Stock keeps red for real scarcity only: "5 left in stock" became a green "5 in stock"; "3 left in stock" stays red. The logo now reads "Gearline Cycles" with a real space.

## 5. Distill (`04-distill.html`)
- The empty hero photo placeholder is hidden on phones: it pushed the deals 200px further down and helped nobody choose a bike. On a 375×812 screen the Hot deals heading now starts at y 833 instead of 1104.
- Removed an unused utility class and pointed the nav's "Deals" link at the deals section instead of nowhere.
- Kept the three price signals (old price, saving, discount tag): the brief asks for a discount badge, and the saving in euros is what the critique found missing.

## 6. Quieter (`05-quieter.html`)
- Removed the 16 corner pin dots and gave the cards back the space they reserved; the bib now reads through its shape, slanted discount tag and tear line alone.
- The card hover keeps its 3px lift but loses the tilt, which suggested the whole card was a link.
- The tear line went from a 2px to a 1px dash, and the hero photo's bike outline is fainter (12% instead of 18% white), so neither competes with prices or headline. Colours, type and the yellow trust band are untouched.

## 7. Harden (`06-harden.html`)
- Sized bikes now show size chips (44px targets) and Add to cart will not proceed without one: it says "Choose a size first.", marks the chips and moves focus to the first available size. Sold-out sizes are struck through, disabled and announced as "sold out" (demo: XL on the Trailblazer G2, consistent with its 3 left).
- Product names clamp to two lines with room reserved for both, and break long words, so a long name never pushes one card's price out of line with its row.
- A product photo that fails to load is removed so the labelled placeholder shows instead of a broken image; a sold-out card state (`.bib.is-soldout`, `.stock.out`) is styled for when a bike runs out. The e-bike, which has no sizes, shows its range in the same slot.

## 8. Adapt (`07-adapt.html`)
- Phones get navigation back: the five categories become a swipeable row of 44px outlined chips under the logo, which runs past the screen edge so it reads as scrollable. Before, the menu simply disappeared below 900px.
- At 375px the headline scales to fit the width (52 to 64px), cards tighten their padding, the price drops to 52px, and single-column cards stop reserving a second line for the name. Logo and cart are 44px tall touch targets.
- Checked at 375×812: no horizontal overflow, Shop all bikes at y 448 to 516, all four trust points end at y 759, and Hot deals starts at y 819.

## 9. Animate (`08-animate.html`)
- One focal moment, Add to cart: a yellow sweep crosses the button like a finish-line flag (320ms, decelerating), the label reads "Added" with a check for 1.8s, and the cart count appears in the header with a short pop. Screen readers hear "Trailblazer G2 Gravel, size M added to cart. 1 item in cart."
- Supporting feedback only: the existing 3px card lift, a 1px press on buttons, and 150ms colour transitions on size chips. No scroll reveals or entrance choreography.
- `prefers-reduced-motion` removes the lift, press, sweep and pop, but keeps the colour change, label change and count, so the feedback survives without movement.

## 10. Polish (`09-polish.html`)
- Every card now stacks the old price and saving on their own line under the price; before, short prices kept them on one line and long ones wrapped, so the four cards no longer matched. Category and discount tag now share a centre line.
- Fixed two defects: the cart count showed "0" before anything was added (its display rule overrode `hidden`), and the rating link's focus ring was yellow on the yellow trust strip, so it was invisible; it is now Tarmac.
- Brought sizes back to the system: the phone-only headline (52 to 64px) and price (52px) overrides from step 8 were off the DESIGN.md type scale, so phones now use the standard tokens (60px minimum headline, 58px price). The mobile hero padding was tightened 8px so the trust strip still ends above the fold (y 803 on 375×812). The trust strip is back to 70px tall on desktop, and on phones the rating drops the word "from" so it stops wrapping onto three lines. The design-system scan is clean (0 findings).

## 11. Audit (`10-audit.html`, final)
- No P0. Two P1s fixed:
  - **Desktop nav targets:** the links were 17px tall, below the 44px rule in PRODUCT.md. They are now 44px.
  - **Cart's screen-reader name:** it read "Cart items" even when empty. It now reads "Cart" until something is added, then "Cart, 1 item".
- P2 fixes:
  - **Size groups:** each is now named for its bike ("Size for Aero R5 Road"), not four identical "Size" groups.
  - **Mobile category chips:** their outline is as visible as the secondary button's.
  - **Phone headline:** its minimum size is 52px, so it stays on four lines at 375px. At 375×812, Shop all bikes now ends at y 493, the trust strip at y 724, and Hot deals starts at y 784, inside the first screen.
- Verified:
  - **Touch targets:** none under 44px at 1440 or 375.
  - **Overflow:** no horizontal overflow at either width.
  - **Contrast:** every text pair passes WCAG AA. The lowest is nav links at 6.4:1.
  - **Keyboard:** the tab order follows the visual order, and radio groups take arrow keys.
  - **Script:** no errors. The size guard, Added state and live announcements work.
  - **Reduced motion:** honoured.
  - **Design-system scan:** 0 findings.
- Left as is: the Archivo request loads the full italic and width ranges (could be subset later), and a few overlay colours on placeholders are hard-coded rgba values.
