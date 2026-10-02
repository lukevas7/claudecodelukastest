---
name: Gearline Cycles (Direction B)
description: Race-programme e-commerce for a fictional bike shop. Cobalt and leader yellow, condensed italic type, deal cards set as race bibs.
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
    fontSize: "clamp(60px, 8.2vw, 124px)"
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
    fontSize: "58px"
    fontWeight: 900
    lineHeight: 0.82
    letterSpacing: "-0.01em"
    fontFeature: "\"tnum\" 1, \"lnum\" 1"
    fontVariation: "\"wdth\" 62"
  price:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "42px"
    fontWeight: 900
    lineHeight: 1
    fontFeature: "\"tnum\" 1, \"lnum\" 1"
    fontVariation: "\"wdth\" 62"
  title:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "26px"
    fontWeight: 800
    lineHeight: 1
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
    fontSize: "13px"
    fontWeight: 800
    letterSpacing: "0.06em"
  caption:
    fontFamily: "Archivo, Arial Narrow, sans-serif"
    fontSize: "14px"
    fontWeight: 500
    lineHeight: 1.35
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
  deal-bib:
    backgroundColor: "{colors.white}"
    textColor: "{colors.tarmac}"
    rounded: "{rounded.md}"
    padding: "16px 16px 30px"
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

The page reads like the printed programme handed out at an amateur race: entries in heavy condensed type, numbers big enough to read from the barrier, and two team colours that never share the job. Cobalt owns the top of the page and yellow carries the facts that close a sale. Below the hero, the deals sit on a cool grey ground as a row of race bibs, each pinned on at four corners, each leading with its number. Here the number is the discount.

The energy is loud but disciplined. Every heavy element sits on a strict grid with one gutter, every card holds the same fields in the same order, and the trust facts run as one straight line rather than a cloud of badges. The italic slant is the only motion in the static layout, and it always leans forward. Type does the shouting; colour and alignment keep it readable.

The source of this system is `bike-shop/hero-b.html`, a hero and Hot deals section built desktop first at 1440px that collapses to a single column at 390px. All content is fictional demo material.

**Key Characteristics:**
- Two fields of colour at page scale: a cobalt hero and a yellow trust strip, with white bibs on paper grey below.
- One family, Archivo, used across its width axis: 62% for display and numerals, 75% for titles and controls, 100% for running text.
- Display type is uppercase, italic and weight 900; running text is never uppercase.
- Numerals are tabular and lining wherever a price or discount appears.
- Deal cards are race bibs: four pin holes, a dashed tear line, the discount as the bib number.

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
- **Tarmac** (`tarmac`): body text on light ground, the discount number, text on yellow, and the Add to cart button at rest.
- **Tarmac Soft** (`tarmac-soft`): the struck old price and photo captions on light plates.
- **White** (`white`): bib surfaces and all text on cobalt.
- **Start Line Grey** (`paper`): the deals section ground, the photo plates inside bibs, and the punched pin holes.
- **Tear Line** (`line`): the dashed rule between price and specs, and the placeholder bike outline on light plates.

### Status
- **Low Stock Red** (`stock-low`): "3 left in stock" and similar counts. Always paired with a dot and the words, never colour alone.
- **In Stock Green** (`stock-ok`): "In stock". Same dot and words pattern.

### Named Rules
**The Two Teams Rule.** Cobalt and yellow each own whole regions; they do not take turns on small elements. Yellow appears on cobalt or as its own field, never as a thin accent on paper grey, except the 3px underline on "View all deals".

**The Price Is Cobalt Rule.** The current price is always Race Cobalt; nothing else at that size and weight uses the colour. The old price is always Tarmac Soft, struck through, and at least 2.5 times smaller.

## Typography

**Display Font:** Archivo at 62% width (fallback Arial Narrow, sans-serif)
**Body Font:** Archivo at 100% width
**Label Font:** Archivo at 75% to 100% width, uppercase, tracked

**Character:** One variable family stretched across its width axis, like the different weights of type on a race programme: compressed and heavy for the names and numbers, normal width for the sentences that explain them.

### Hierarchy
- **Display** (900 italic, uppercase, `display` size, line height 0.86): the hero headline only. The second sentence is set in Leader Yellow on its own line, and "48 hours" never breaks across lines.
- **Headline** (900 italic, uppercase, `headline` size, line height 0.9): section titles such as "Hot deals", in Race Cobalt.
- **Discount** (900, 58px, 62% width, tabular): the bib number. The largest figure on each card.
- **Price** (900, 42px, 62% width, tabular): the current price, in Race Cobalt.
- **Title** (800, 26px, 75% width, uppercase): product names on bibs.
- **Wordmark** (900 italic, 30px, 62% width, uppercase): the logo, and the 4.8/5 figure in the trust strip. **Wordmark Small** (24px) replaces it on phones.
- **Button Label** (900, 22px, 75% width, uppercase, 0.02em tracking): the primary button only.
- **Control** (700, 17px): the secondary button label.
- **Lede** (500, 20px, line height 1.45, max 30ch): the supporting line under the headline. Under 900px it uses **Lede Small** (18px).
- **Body** (400, 16px, line height 1.45): running text and spec lines (spec lines use 600 at 14px).
- **Caption** (500, 14px, line height 1.35): photo placeholder captions and spec lines (spec lines at 600). The bib plate caption is the one 12.5px exception.
- **Label** (700, 15px, uppercase, 0.04em tracking): nav links, the cart link, "View all deals" (800).
- **Label Small** (800, 13px, uppercase, 0.06em tracking): the category on each bib.

### Named Rules
**The Lean Forward Rule.** Italic is reserved for display and headline sizes and the logo. Below 26px, type stands upright.

**The Narrow Numbers Rule.** Prices, discounts and the 4.8/5 rating are set at 62% width with tabular lining figures, so a column of prices lines up and a discount reads at a glance. Struck old prices drop the tabular setting so the comma does not float.

## Layout

A single page gutter (`gutter`, 18px at phone width up to 64px at 1440px) frames every row: nav, hero, photo, trust strip and deals all start on the same left edge.

- **Hero:** a two-column grid at 7fr and 5fr with a 56px gap. The left column holds the whole message as one vertically centred group: headline, then the lede 28px below, then the two buttons 32px below that. The right column is the photo, stretched to the full height of the message (at least 360px). The trust strip runs the full width directly under the hero, as four equal columns.
- **Deals:** a header row with the headline left and "View all deals" right, aligned to the baseline, then a four-column grid with a 24px gap. Section padding is 80px above and 104px below.
- **Rhythm:** 6, 12, 16, 24 and 40px steps inside components; 80 and 104px between sections. More space above a heading than below it.
- **Under 1180px:** deals and trust strip drop to two columns.
- **Under 900px:** nav links hide (logo and cart stay). The hero becomes one column in this order: headline, lede, buttons, trust strip, then the photo, so the trust facts stay above the fold on a phone. The photo drops to 200px tall.
- **Under 560px:** buttons stack full width, the trust strip becomes one column with hairline dividers, and deals become one column.

### Named Rules
**The One Column Pitch Rule.** Headline, lede and primary button live in one column, in that order, with nothing between them. Images support from the side or below; they never sit between the promise and the action.

## Elevation & Depth

Mostly flat colour fields; depth appears only on the bibs, which sit on the page like card stock with a soft, offset shadow. The yellow strip and cobalt hero use no shadow at all.

### Shadow Vocabulary
- **Bib rest** (`box-shadow: 0 1px 2px rgba(13,15,26,.08), 0 10px 24px -14px rgba(13,15,26,.25)`): every deal card at rest.
- **Bib lift** (`box-shadow: 0 2px 4px rgba(13,15,26,.08), 0 20px 34px -16px rgba(13,15,26,.35)`): on hover, together with a 3px rise and a -0.4 degree turn, as if the bib lifted at one corner.
- **Pin hole** (`box-shadow: inset 0 1px 2px rgba(13,15,26,.25)`): the four punched holes, filled with Start Line Grey.

### Named Rules
**The Only Bibs Lift Rule.** Shadows belong to the bibs. Fields, strips, buttons and photos stay flat; a button shows hover by colour or a short slide, not by elevation.

## Shapes

Hard edges for anything that carries the brand, soft corners only on things you would hold.

- **Square and slanted:** both hero buttons are rectangles skewed by -8 degrees with their content counter-skewed upright. The logo's yellow block, the trust strip and the hero photo are square.
- **Soft:** bibs have 10px corners. Photo plates inside bibs and the Add to cart button have 4px corners.
- **Punched:** four 10px circles, 10px in from each bib corner.
- **Torn:** a 2px dashed rule in Tear Line separates price from specs on every bib.
- **Flat placeholders:** photo areas are flat fields of colour with a faint bike outline and a caption chip until real photography replaces them. No stripes, hatching or gradients.

## Components

### Buttons
Loud, heavy and few. A hero has one yellow button and one outlined button, never more.

- **Shape:** rectangle, no radius, skewed -8 degrees; content counter-skewed to stay upright.
- **Primary ("Shop bikes"):** Leader Yellow fill, Tarmac text at 900, 75% width, uppercase, 22px, padding 18px 34px, 60px tall, trailing arrow.
- **Primary hover:** Leader Yellow Hover, slides 3px right (250ms, `cubic-bezier(.2,.8,.2,1)`).
- **Secondary ("Find my bike"):** transparent with a 2px border at 50% white, white text at 700 and 17px, a target icon before the label, 60px tall. Hover takes the border to full white.
- **Add to cart:** full card width, 52px tall, 4px corners, Tarmac fill, white uppercase 800 text tracked 0.06em, cart icon. Hover swaps to Leader Yellow fill with Tarmac text.
- **Focus:** 3px Leader Yellow outline, 3px offset, on cobalt; 3px Race Cobalt outline inside the deals section.

### Race Bib (deal card)
The signature component. Every bib holds the same fields in the same order so a row of four scans like a start list.

- **Surface:** white, 10px corners, padding 16px 16px 30px, bib rest shadow, four pin holes.
- **Top row:** category in Label Small and Race Cobalt on the left; the discount as the bib number on the right ("−17%").
- **Plate:** a 3:2 photo area on Start Line Grey with 4px corners and a white caption chip naming the shot.
- **Then:** product name (Title), current price in Race Cobalt with the struck old price beside it, a dashed tear line, one row with the key spec on the left and stock status on the right, and the Add to cart button.
- **Stock status:** an 8px dot plus the words, 800 weight, in Low Stock Red or In Stock Green.

### Trust Strip
- **Style:** a full-width Leader Yellow band directly under the hero, Tarmac text at 700 and 16px, four equal columns, each led by a 26px stroke icon.
- **Rating:** "4.8/5" set as a 30px narrow numeral after a filled star, then the review count.

### Navigation
- **Logo:** "GEARLINE" in Tarmac on a Leader Yellow block, then "CYCLES" in white, both 900 italic, 62% width, uppercase, 30px (24px on phones).
- **Links:** uppercase Label in white at 86% opacity; hover goes to full opacity with a 2px underline 6px below.
- **Cart:** cart icon plus "CART", always visible. Links hide under 900px.

### Image Placeholder
- **Style:** a flat field (Cobalt Deep on the hero, Start Line Grey in bibs) with a faint bike outline and a caption chip that names the shot, for example "Product photo: gravel bike, side view". Replace with real photography; keep the caption as the image's alt text.

## Do's and Don'ts

### Do:
- **Do** keep the hero to one primary action in Leader Yellow and one outlined secondary.
- **Do** set every price and discount in the narrow 900 weight with tabular figures, current price in Race Cobalt.
- **Do** keep bib fields in the fixed order: category and discount, plate, name, price, tear line, spec and stock, button.
- **Do** keep the trust strip directly under the hero at every width, ahead of the photo on phones.
- **Do** pair every stock colour with a dot and words.
- **Do** align every row to the single page gutter (`gutter`).

### Don't:
- **Don't** use yellow as small accent text on Start Line Grey or white; it fails contrast and breaks the Two Teams Rule.
- **Don't** set running text or anything under 26px in italic or uppercase, except labels.
- **Don't** add shadows to fields, strips or buttons; only bibs lift.
- **Don't** round the hero buttons or remove their slant.
- **Don't** add countdown timers or other fake urgency; stock counts are the only scarcity signal and must be true.
- **Don't** use emoji, gradient blobs, glows, glass effects or decorative stripe patterns.
