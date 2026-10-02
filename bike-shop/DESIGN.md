---
name: Gearline Cycles (Direction B)
description: Race-programme e-commerce for a fictional bike shop. Cobalt and leader yellow, condensed italic type, deal cards set as race bibs that lead with the price.
colors:
  cobalt: "#1636D9"
  cobalt-deep: "#0E248F"
  cobalt-ink: "#0A1A66"
  yellow: "#FFE135"
  yellow-hover: "#FFEB70"
  white: "#FFFFFF"
  tarmac: "#0D0F1A"
  tarmac-soft: "#4A4F66"
  paper: "#ECEEF5"
  line: "#D3D7E6"
  stock-low: "#B3261E"
  stock-ok: "#11703F"
typography:
  display:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "clamp(52px, 8.2vw, 124px)"
    fontWeight: 900
    lineHeight: 0.86
    letterSpacing: "-0.01em"
    fontVariation: "\"wdth\" 62"
  headline:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "clamp(52px, 6vw, 88px)"
    fontWeight: 900
    lineHeight: 0.9
    fontVariation: "\"wdth\" 62"
  discount:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "24px"
    fontWeight: 900
    lineHeight: 1
    fontFeature: "\"tnum\" 1, \"lnum\" 1"
    fontVariation: "\"wdth\" 62"
  price:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "58px"
    fontWeight: 900
    lineHeight: 0.9
    letterSpacing: "-0.01em"
    fontFeature: "\"tnum\" 1, \"lnum\" 1"
    fontVariation: "\"wdth\" 62"
  title:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "24px"
    fontWeight: 800
    lineHeight: 1.05
    fontVariation: "\"wdth\" 75"
  wordmark:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "30px"
    fontWeight: 900
    lineHeight: 1
    letterSpacing: "0.01em"
    fontVariation: "\"wdth\" 62"
  wordmark-small:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "24px"
    fontWeight: 900
    lineHeight: 1
    fontVariation: "\"wdth\" 62"
  button-label:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "22px"
    fontWeight: 900
    letterSpacing: "0.02em"
    fontVariation: "\"wdth\" 75"
  control:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "17px"
    fontWeight: 700
  lede:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "20px"
    fontWeight: 500
    lineHeight: 1.45
  lede-small:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "18px"
    fontWeight: 500
    lineHeight: 1.45
  body:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.45
  label:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "15px"
    fontWeight: 700
    letterSpacing: "0.04em"
  label-small:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "14px"
    fontWeight: 800
    letterSpacing: "0.06em"
  caption:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "14px"
    fontWeight: 500
    lineHeight: 1.35
  caption-small:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "13px"
    fontWeight: 500
    lineHeight: 1.3
rounded:
  none: "0px"
  xs: "4px"
  md: "10px"
  full: "50%"
spacing:
  gutter: "clamp(18px, 4.5vw, 64px)"
  xs: "6px"
  sm: "12px"
  md: "16px"
  lg: "24px"
  xl: "40px"
  section: "80px"
  section-end: "104px"
components:
  button-primary:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.tarmac}"
    typography: "{typography.button-label}"
    rounded: "{rounded.none}"
    padding: "18px 34px"
    height: "60px"
  button-primary-hover:
    backgroundColor: "{colors.yellow-hover}"
    textColor: "{colors.tarmac}"
  button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.white}"
    typography: "{typography.control}"
    rounded: "{rounded.none}"
    padding: "16px 20px"
    height: "60px"
  button-cart:
    backgroundColor: "{colors.tarmac}"
    textColor: "{colors.white}"
    typography: "{typography.label}"
    rounded: "{rounded.xs}"
    height: "52px"
    width: "100%"
  button-cart-hover:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.tarmac}"
  button-cart-added:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.tarmac}"
  deal-bib:
    backgroundColor: "{colors.white}"
    textColor: "{colors.tarmac}"
    rounded: "{rounded.md}"
    padding: "16px 16px 20px"
  discount-tag:
    backgroundColor: "{colors.tarmac}"
    textColor: "{colors.yellow}"
    typography: "{typography.discount}"
    rounded: "{rounded.none}"
    padding: "6px 10px 4px"
  size-chip:
    backgroundColor: "{colors.white}"
    textColor: "{colors.tarmac}"
    rounded: "{rounded.xs}"
    padding: "0 10px"
    height: "44px"
  size-chip-selected:
    backgroundColor: "{colors.cobalt}"
    textColor: "{colors.white}"
  size-chip-sold-out:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.tarmac-soft}"
  cart-count:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.tarmac}"
    rounded: "{rounded.xs}"
    height: "22px"
  nav-chip-mobile:
    backgroundColor: "transparent"
    textColor: "{colors.white}"
    rounded: "{rounded.none}"
    padding: "0 16px"
    height: "44px"
  product-plate:
    backgroundColor: "{colors.paper}"
    rounded: "{rounded.xs}"
  trust-strip:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.tarmac}"
    typography: "{typography.label}"
    padding: "20px 0"
  nav-bar:
    backgroundColor: "{colors.cobalt}"
    textColor: "{colors.white}"
    typography: "{typography.label}"
    padding: "22px 0"
  image-label:
    backgroundColor: "{colors.cobalt-ink}"
    textColor: "#E4E8FF"
    typography: "{typography.caption}"
    padding: "10px 14px"
---

# Design System: Gearline Cycles (Direction B)

## Overview

**Creative North Star: "The Start List"**

The page reads like the printed programme handed out at an amateur race: entries in heavy condensed type, numbers big enough to read from the barrier, and two team colours that never share the job. Cobalt owns the top of the page and yellow carries the facts that close a sale. Below the hero, the deals sit on a cool grey ground as a row of race bibs. Each bib leads with the number that matters most to a buyer, the price, and carries its discount as a small slanted tag.

The energy is loud but disciplined. Every heavy element sits on a strict grid with one gutter, every card holds the same fields in the same order, and the trust facts run as one straight line rather than a cloud of badges. The italic slant is the only motion in the static layout, and it always leans forward. Type does the shouting; colour and alignment keep it readable.

The source of this system is `bike-shop/hero-b.html`, a hero and Hot deals section built desktop first at 1440px that collapses to a single column at 390px. All content is fictional demo material.

**Key Characteristics:**
- Two fields of colour at page scale: a cobalt hero and a yellow trust strip, with white bibs on paper grey below.
- One family, Archivo, used across its width axis: 62% for display and numerals, 75% for titles and controls, 100% for running text.
- Display type is uppercase, italic and weight 900; running text is never uppercase.
- Numerals are tabular and lining wherever a price or discount appears.
- Deal cards are race bibs: price as the biggest figure, a slanted discount tag, a dashed tear line, size chips, and one Add to cart button.

## Colors

Two saturated team colours on a cool, near-neutral ground, with a near-black that reads like fresh tarmac.

### Primary
- **Race Cobalt** (`cobalt`): the hero field, the Hot deals headline, every current price, and the category label on each bib. It is the colour of the brand and of the number you pay.
- **Cobalt Deep** (`cobalt-deep`): the hero photo field, one step darker so the image area separates from the hero ground without a border.
- **Cobalt Ink** (`cobalt-ink`): the caption chip on dark photo placeholders.

### Secondary
- **Leader Yellow** (`yellow`): the primary action, the trust strip, the yellow block behind "Gearline" in the logo, the second line of the headline, the underline on "View all deals", the cart button's hover, focus rings on cobalt, and text selection.
- **Leader Yellow Hover** (`yellow-hover`): the lighter yellow of the primary button on hover.

### Neutral
- **Tarmac** (`tarmac`): body text on light ground, the discount tag, the "Save" label, text on yellow, and the Add to cart button at rest.
- **Tarmac Soft** (`tarmac-soft`): the struck old price, the "Size" and "Range" labels, sold-out sizes, and photo captions on light plates.
- **White** (`white`): bib surfaces and all text on cobalt.
- **Start Line Grey** (`paper`): the deals section ground, the photo plates inside bibs, and the fill of sold-out size chips.
- **Tear Line** (`line`): the dashed rule between price and size, the border of size chips at rest, and the placeholder bike outline on light plates.

### Status
- **Low Stock Red** (`stock-low`): counts of 3 or fewer ("3 left in stock") and the "Choose a size first." message. Always paired with a dot or words, never colour alone; larger counts are In Stock Green ("5 in stock") so red keeps its meaning.
- **In Stock Green** (`stock-ok`): "In stock". Same dot and words pattern.

### Named Rules
**The Two Teams Rule.** Cobalt and yellow each own whole regions; they do not take turns on small elements. Yellow appears on cobalt or as its own field, never as a thin accent on paper grey, except the 3px underline on "View all deals".

**The Price Is Cobalt Rule.** The current price is always Race Cobalt and the largest figure on its card; nothing else at that size and weight uses the colour. The old price is Tarmac Soft, struck through, on its own line with the saving in euros beside it.

## Typography

**Display Font:** Archivo at 62% width (fallback Arial Narrow, sans-serif)
**Body Font:** Archivo at 100% width
**Label Font:** Archivo at 75% to 100% width, uppercase, tracked

**Character:** One variable family stretched across its width axis, like the different weights of type on a race programme: compressed and heavy for the names and numbers, normal width for the sentences that explain them.

### Hierarchy
- **Display** (900 italic, uppercase, `display` size, line height 0.86): the hero headline only. The second sentence is set in Leader Yellow on its own line, and "48 hours" never breaks across lines.
- **Headline** (900 italic, uppercase, `headline` size, line height 0.9): section titles such as "Hot deals", in Race Cobalt.
- **Price** (900, 58px, 62% width, tabular, line height 0.9): the current price, in Race Cobalt. The largest figure on each card, at every width.
- **Discount** (900, 24px, 62% width, tabular): the discount tag, Leader Yellow on Tarmac, slanted -8 degrees like the buttons. Under it, the old price (600, 18px, tabular) and the saving ("SAVE €400", 800, 15px, uppercase, Tarmac) share one line.
- **Title** (800, 24px, 75% width, uppercase, line height 1.05): product names on bibs, clamped to two lines with both lines reserved when cards sit side by side.
- **Wordmark** (900 italic, 30px, 62% width, uppercase): the logo, and the 4.8/5 figure in the trust strip. **Wordmark Small** (24px) replaces it on phones.
- **Button Label** (900, 22px, 75% width, uppercase, 0.02em tracking): the primary button only.
- **Control** (700, 17px): the secondary button label.
- **Lede** (500, 20px, line height 1.45, max 30ch): the supporting line under the headline. Under 900px it uses **Lede Small** (18px).
- **Body** (400, 16px, line height 1.45): running text and spec lines (spec lines use 600 at 14px).
- **Caption** (500, 14px, line height 1.35): photo placeholder captions on the hero and the stock line (stock at 800, 15px). The bib plate caption and the cart count use **Caption Small** (13px).
- **Label** (700, 15px, uppercase, 0.04em tracking): nav links, the cart link, "View all deals" (800).
- **Label Small** (800, 14px, uppercase, 0.06em tracking): the category on each bib and the "Size" and "Range" labels.

### Named Rules
**The Price Leads Rule.** On a product, the order of emphasis is price, then saving, then name. No discount, badge or headline inside a card may be larger than its price.

**The Lean Forward Rule.** Italic is reserved for display and headline sizes and the logo. Below 26px, type stands upright.

**The Narrow Numbers Rule.** Prices, discounts and the 4.8/5 rating are set at 62% width with tabular lining figures, so a column of prices lines up and a discount reads at a glance. Old prices keep tabular figures too.

## Layout

A single page gutter (`gutter`, 18px at phone width up to 64px at 1440px) frames every row: nav, hero, photo, trust strip and deals all start on the same left edge.

- **Hero:** a two-column grid at 7fr and 5fr with a 56px gap. The left column holds the whole message as one vertically centred group: headline, then the lede 28px below, then the two buttons 32px below that. The right column is the photo, stretched to the full height of the message (at least 360px). The trust strip runs the full width directly under the hero, as four equal columns.
- **Deals:** a header row with the headline left and "View all deals" right, aligned to the baseline, then a four-column grid with a 24px gap. Section padding is 80px above and 104px below. Inside a bib the reading order is photo, category and discount tag, name, price, old price and saving, size (or range), stock, then the Add to cart button pinned to the bottom, so prices and buttons line up across a row.
- **Rhythm:** 6, 12, 16, 24 and 40px steps inside components; 80 and 104px between sections. More space above a heading than below it.
- **Under 1180px:** deals and trust strip drop to two columns.
- **Under 900px:** the category links become a row of 44px outlined chips under the logo that scrolls sideways past the screen edge. The hero becomes one column in this order: headline, lede, buttons, then the trust strip; the empty hero photo placeholder is hidden on phones so the deals come up sooner.
- **Under 560px:** buttons stack full width, the trust strip becomes a 2×2 grid (14px text, the rating drops "from"), deals become one column and names stop reserving a second line. At 375×812 the trust strip ends at y 724 and Hot deals starts at y 784.

### Named Rules
**The One Column Pitch Rule.** Headline, lede and primary button live in one column, in that order, with nothing between them. Images support from the side or below; they never sit between the promise and the action.

## Elevation & Depth

Mostly flat colour fields; depth appears only on the bibs, which sit on the page like card stock with a soft, offset shadow. The yellow strip and cobalt hero use no shadow at all.

### Shadow Vocabulary
- **Bib rest** (`box-shadow: 0 1px 2px rgba(13,15,26,.08), 0 10px 24px -14px rgba(13,15,26,.25)`): every deal card at rest.
- **Bib lift** (`box-shadow: 0 2px 4px rgba(13,15,26,.08), 0 20px 34px -16px rgba(13,15,26,.35)`): on hover, together with a 3px rise. No tilt: only the button inside is clickable.

### Named Rules
**The Only Bibs Lift Rule.** Shadows belong to the bibs. Fields, strips, buttons and photos stay flat; a button shows hover by colour or a short slide, not by elevation.

## Shapes

Hard edges for anything that carries the brand, soft corners only on things you would hold.

- **Square and slanted:** both hero buttons are rectangles skewed by -8 degrees with their content counter-skewed upright. The logo's yellow block, the trust strip and the hero photo are square.
- **Soft:** bibs have 10px corners. Photo plates, size chips, the cart count and the Add to cart button have 4px corners.
- **Slanted:** the discount tag is skewed -8 degrees, the same lean as the hero buttons.
- **Torn:** a 1px dashed rule in Tear Line separates price from size on every bib. It is the only bib ornament; the corner pin holes were removed.
- **Flat placeholders:** photo areas are flat fields of colour with a faint bike outline and a caption chip until real photography replaces them. No stripes, hatching or gradients.

## Components

### Buttons
Loud, heavy and few. A hero has one yellow button and one outlined button, never more.

- **Shape:** rectangle, no radius, skewed -8 degrees; content counter-skewed to stay upright.
- **Primary ("Shop all bikes"):** Leader Yellow fill, Tarmac text at 900, 75% width, uppercase, 22px, padding 18px 34px, 60px tall, trailing arrow.
- **Primary hover:** Leader Yellow Hover, slides 3px right (250ms, `cubic-bezier(.2,.8,.2,1)`).
- **Secondary ("Find my bike"):** transparent with a 2px border at 50% white, white text at 700 and 17px, a target icon before the label, 60px tall. Hover takes the border to full white.
- **Add to cart:** full card width, 52px tall, 4px corners, Tarmac fill, white uppercase 800 text tracked 0.06em, cart icon. Hover swaps to Leader Yellow fill with Tarmac text.
- **Focus:** 3px Leader Yellow outline, 3px offset, on cobalt; 3px Race Cobalt outline inside the deals section.

### Race Bib (deal card)
The signature component. Every bib holds the same fields in the same order so a row of four scans like a start list, and the price is always the loudest thing on it.

- **Surface:** white, 10px corners, padding 16px 16px 20px, bib rest shadow. No pin holes.
- **Plate first:** a 3:2 photo area on Start Line Grey with 4px corners and a white caption chip naming the shot. A real `<img>` covers it; if the image fails to load it is removed and the placeholder shows.
- **Then:** category (Label Small, Race Cobalt) with the discount tag on the right; product name (Title, two lines max); price (Price) with the old price and "Save €X" on the line below; a dashed tear line; size chips (or the range for one-size e-bikes); the stock line; the Add to cart button.
- **Stock status:** an 8px dot plus the words, 800 weight, 15px. Low Stock Red for 3 or fewer ("3 left in stock"), In Stock Green otherwise ("In stock", "5 in stock"), Tarmac Soft for "Sold out".
- **Size chips:** a radio group with a "Size" legend (named for the bike for screen readers). Chips are 44px tall, 2px Tear Line border, 4px corners; selected is Race Cobalt with white text; sold-out sizes are struck through on Start Line Grey, disabled, and announced as "sold out".
- **Add to cart:** a sized bike without a size chosen does not go in the cart: the message "Choose a size first." appears in Low Stock Red, the chips' borders turn red and focus moves to the first available size. On success a yellow sweep crosses the button left to right (320ms, `cubic-bezier(.16,1,.3,1)`), the label reads "Added" with a check for 1.8s, the header cart count pops in, and a live region announces "Trailblazer G2 Gravel, size M added to cart. 1 item in cart." Reduced motion keeps the colour, label and count changes without the movement.
- **Sold out:** `.bib.is-soldout` greys the price to Tarmac Soft and the stock line reads "Sold out".

### Trust Strip
- **Style:** a full-width Leader Yellow band directly under the hero, Tarmac text at 700 and 16px, four equal columns, each led by a 26px stroke icon.
- **Rating:** "4.8/5" set as a 30px narrow numeral after a filled star, then "from 2,300 reviews", the whole row one link to the reviews. Its focus ring is Tarmac, because yellow would vanish on the strip.
- **Wording:** "Free delivery on orders over €500", "30-day returns", "2-year warranty".

### Navigation
- **Logo:** "GEARLINE" in Tarmac on a Leader Yellow block, then "CYCLES" in white, both 900 italic, 62% width, uppercase, 30px (24px on phones).
- **Links:** uppercase Label in white at 86% opacity, 44px tall hit areas; hover goes to full opacity with a 2px underline 6px below.
- **Cart:** cart icon plus "CART", always visible, 44px tall. A yellow count badge (4px corners, Tarmac numerals) appears after the first add and pops on each change; screen readers hear "Cart" or "Cart, 2 items".
- **Phones:** under 900px the category links become a sideways-scrolling row of 44px chips with a 2px white outline at 50%.

### Image Placeholder
- **Style:** a flat field (Cobalt Deep on the hero, Start Line Grey in bibs) with a faint bike outline and a caption chip that names the shot, for example "Product photo: gravel bike, side view". Replace with real photography; keep the caption as the image's alt text.

## Do's and Don'ts

### Do:
- **Do** keep the hero to one primary action in Leader Yellow and one outlined secondary.
- **Do** set every price and discount in the narrow 900 weight with tabular figures, current price in Race Cobalt.
- **Do** keep bib fields in the fixed order: plate, category and discount tag, name, price, old price and saving, size or range, stock, button.
- **Do** keep the trust strip directly under the hero at every width, ahead of the photo on phones.
- **Do** pair every stock colour with a dot and words.
- **Do** align every row to the single page gutter (`gutter`).

- **Do** make the price the largest figure on every card and state the saving in euros next to the old price.
- **Do** give every sized product size chips and block Add to cart until a size is chosen.

### Don't:
- **Don't** use yellow as small accent text on Start Line Grey or white; it fails contrast and breaks the Two Teams Rule.
- **Don't** set running text or anything under 26px in italic or uppercase, except labels.
- **Don't** add shadows to fields, strips or buttons; only bibs lift, and they never tilt.
- **Don't** bring back corner pin holes or other ornament on the bibs; the tag, the tear line and the shape carry the race-bib idea.
- **Don't** use red for stock counts above 3.
- **Don't** round the hero buttons or remove their slant.
- **Don't** add countdown timers or other fake urgency; stock counts are the only scarcity signal and must be true.
- **Don't** use emoji, gradient blobs, glows, glass effects or decorative stripe patterns.
