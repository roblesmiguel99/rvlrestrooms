---
name: Royal Valley Luxury Restrooms
description: A boutique hotel suite you can tow; bottle-green lobby, linen card stock, brass hardware.
colors:
  lobby: "#13322b"
  lobby-deep: "#0b221d"
  lobby-2: "#1b4037"
  linen: "#ebe6dc"
  linen-2: "#ddd6c8"
  ink: "#16261f"
  ink-dim: "#4a564f"
  text: "#ece7dd"
  text-dim: "#b7c4b9"
  brass: "#b9925a"
  brass-hi: "#e0c591"
  brass-lo: "#7f6237"
  brass-ink: "#6a5130"
  oxblood: "#7a2e2e"
  rule: "rgba(185,146,90,.38)"
typography:
  display:
    fontFamily: "Gilda Display, Didot, serif"
    fontSize: "clamp(2.7rem, 5.6vw, 4.9rem)"
    fontWeight: 400
    lineHeight: 1.06
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Gilda Display, Didot, serif"
    fontSize: "clamp(2.2rem, 4.8vw, 3.9rem)"
    fontWeight: 400
    lineHeight: 1.06
    letterSpacing: "-0.005em"
  title:
    fontFamily: "Gilda Display, Didot, serif"
    fontSize: "clamp(1.35rem, 2.2vw, 1.7rem)"
    fontWeight: 400
    lineHeight: 1.2
  plate:
    fontFamily: "Marcellus SC, Trajan Pro, serif"
    fontSize: "1.15rem"
    fontWeight: 400
    lineHeight: 1
    letterSpacing: "0.16em"
  body:
    fontFamily: "Hanken Grotesk, Helvetica Neue, Arial, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.65
  label:
    fontFamily: "Hanken Grotesk, Helvetica Neue, Arial, sans-serif"
    fontSize: "0.74rem"
    fontWeight: 500
    lineHeight: 1
    letterSpacing: "0.14em"
  button:
    fontFamily: "Hanken Grotesk, Helvetica Neue, Arial, sans-serif"
    fontSize: "0.78rem"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "0.16em"
rounded:
  card: "3px"
  plate: "4px"
  photo: "6px"
  pill: "999px"
spacing:
  gutter: "clamp(16px, 4vw, 56px)"
  section: "clamp(80px, 11vw, 150px)"
  column-gap: "clamp(28px, 6vw, 96px)"
  list-row: "22px"
  control-gap: "12px"
components:
  button-brass:
    backgroundColor: "{colors.brass}"
    textColor: "{colors.lobby-deep}"
    typography: "{typography.button}"
    rounded: "{rounded.plate}"
    padding: "0.85em 1.5em"
    height: "48px"
  button-brass-hover:
    backgroundColor: "{colors.brass-hi}"
    textColor: "{colors.lobby-deep}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.text}"
    typography: "{typography.button}"
    rounded: "{rounded.plate}"
    padding: "0.85em 1.5em"
    height: "48px"
  button-ink:
    backgroundColor: "{colors.lobby}"
    textColor: "{colors.text}"
    typography: "{typography.button}"
    rounded: "{rounded.plate}"
    padding: "0.85em 1.5em"
    height: "48px"
  button-ink-hover:
    backgroundColor: "{colors.lobby-2}"
    textColor: "{colors.text}"
  fact-chip:
    backgroundColor: "rgba(185,146,90,.12)"
    textColor: "{colors.brass-hi}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "9px 14px"
  linen-card:
    backgroundColor: "{colors.linen}"
    textColor: "{colors.ink}"
    rounded: "{rounded.card}"
    padding: "clamp(28px, 4vw, 56px)"
  field-input:
    backgroundColor: "rgba(255,255,255,.55)"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    padding: "12px"
  station-no-plate:
    backgroundColor: "{colors.brass}"
    textColor: "{colors.lobby-deep}"
    typography: "{typography.plate}"
    rounded: "2px"
    padding: "5px 12px 4px"
---

# Design System: Royal Valley Luxury Restrooms

## Overview

**Creative North Star: "The Suite You Can Tow"**

The page is a boutique hotel lobby that happens to be a restroom trailer. The ground is a drenched bottle-green wall with a faint vertical stripe; everything the guest handles is an object from a good hotel: a die-cut door hanger with a real hole, a turndown card, a check-in slip, a registration card, numbered brass door plates, key-tag fobs on a tether. The furniture of the world (linen card stock, brass hardware, oxblood for the "do not disturb" side) does the persuading; the photographs prove it is real.

Density is generous and hotel-quiet: long section padding, two-column asymmetric grids, one idea per section. Type is a high-contrast display serif against a plain grotesk, with engraved small caps reserved for things that would be stamped or engraved on a plate. Motion is physical and short-lived: a hanger that sways once on load and flips on its axis, door signs that flip on hover, tags that tilt on their tether.

The build explicitly rejects the dark-photo-hero plus gold-icon-columns rental template: photographs sit inside framed "doors" and next to paper objects, never full-bleed behind centered copy.

**Key Characteristics:**
- Bottle-green lobby ground, alternating plain deep sections with the striped lobby wall.
- Linen card-stock objects carry the content that matters: amenities, requirements, booking.
- Brass is hardware, never decoration: buttons, plates, rings, rules, icon strokes.
- Oxblood appears only for the occupied/reserved state and required/error signals.
- Gilda Display for voice, Marcellus SC for engraving, Hanken Grotesk for everything functional.

## Colors

A drenched dark-green ground with one warm metal and one paper; oxblood is a state color, not an accent.

### Primary
- **Hotel Brass** (`brass`): the push-plate button fill, numbered door plates, icon strokes in the contact list, footer column labels, key-tag rings and tethers. Hairline rules are this same brass at 38% (`rule`) or 16–22% for section borders.
- **Polished Brass** (`brass-hi`): hover state of brass, emphasized words inside display headlines and the About pull-line, value names, fact-chip text, the focus ring.
- **Aged Brass** (`brass-lo`): crests and line icons printed on linen card stock, where full brass would be too light to read.

### Secondary
- **Linen Card Stock** (`linen` to `linen-2`): always used as a top-to-bottom gradient between the two, for every paper object (door hanger front, turndown card, check-in slip, registration card). Never used as a flat page background.

### Tertiary
- **Oxblood** (`oxblood`): the RESERVED face of the door hanger and the OCCUPIED face of the mini station signs; required-field asterisks, field error text and the invalid-field border; the input caret.

### Neutral
- **Lobby Green** (`lobby`): the page ground and the striped `lobby-wall` sections; also the fill of the ink button and the VACANT mini sign.
- **Night Lobby** (`lobby-deep`): alternating plain sections (Stations, Requirements, About, footer), the sticky header at 88% with blur, text on brass.
- **Lobby Shade** (`lobby-2`): ink-button hover and scrollbar thumb.
- **Lobby Text** (`text`) / **Lobby Text Dim** (`text-dim`): primary and secondary copy on green.
- **Ink** (`ink`) / **Ink Dim** (`ink-dim`): primary and secondary copy on linen.
- **Brass Ink** (`brass-ink`): the italic sign-off line on linen objects ("With compliments", "Royal Valley").

### Named Rules
**The Hardware Rule.** Brass marks things you press, read a number from, or hang something on. If an element is not hardware, a rule, or an icon stroke, it is not brass.

**The Do Not Disturb Rule.** Oxblood means occupied, reserved, required, or wrong. It never decorates.

**The Paper Gradient Rule.** Linen objects are always `linen` to `linen-2` top to bottom with a 1px inset keyline 10px in; a flat linen rectangle reads as a web card, not card stock.

## Typography

**Display Font:** Gilda Display (with Didot, serif)
**Plate Font:** Marcellus SC (with Trajan Pro, serif)
**Body Font:** Hanken Grotesk (with Helvetica Neue, Arial, sans-serif)

**Character:** A slender hotel-letterhead serif speaks; engraved small caps label the hardware; a neutral grotesk does the logistics so the luxury never gets in the way of a phone number.

### Hierarchy
- **Display** (400, `clamp(2.7rem,5.6vw,4.9rem)`, 1.06): the hero headline only. One phrase may be set in polished brass, upright (never italic).
- **Headline** (400, `clamp(2.2rem,4.8vw,3.9rem)`, 1.06): section h2s, balanced wrap. Linen-object headings step down (`clamp(1.7rem,3vw,2.3rem)` to `clamp(2rem,3.8vw,3rem)`).
- **Title** (400, `clamp(1.35rem,2.2vw,1.7rem)`, 1.2): item names on linen objects, FAQ questions, spec values, contact values. Always Gilda, never bold.
- **Plate** (Marcellus SC, `.14–.16em` tracking, line-height 1): VACANT/RESERVED, "No. n" door plates, value names. Only text that would be engraved or stamped.
- **Body** (400, 1.0625rem, 1.65): paragraphs capped at 62ch; ledes at 44ch, `text-wrap: pretty`.
- **Label** (500–600, `.64–.78rem`, `.12–.22em`, uppercase): buttons, key tags, fact chips, field labels, spec terms, contact-type labels, footer column heads.

### Named Rules
**The Engraving Rule.** Marcellus SC is for words that would physically be engraved on brass or printed on a sign. Headings and body never use it.

**The Tabular Phone Rule.** Every phone number and measurement carries `lining-nums tabular-nums`; numbers are the conversion path.

## Layout

A single centered column `min(1240px, 100%)` with a fluid gutter (`gutter`). Sections alternate between the striped lobby wall and plain night-lobby bands separated by 1px brass hairlines at ~20%, with vertical padding of `section`. Content inside sections uses asymmetric two-column grids (ratios like 0.85 / 1.15 or 1 / 1.05) with `column-gap`, text on one side and a paper object or framed photo on the other. The gallery is a 12-column grid with deliberately unequal spans and aspect ratios (7/5 split over 5/7). Lists are separated by hairline rules with `list-row` padding, never boxed.

Responsive: the key-tag nav collapses to a Menu pill at 1040px; the hero stacks at 900px (the hanger moves to hang on the photo's left edge), and drops above the photo at 480px; two-column section grids stack at 860px; the three station doors stay three-across down to mobile, losing their captions at 760px. Paper objects lose their tilt at narrow widths. Header is sticky at 76px; anchors scroll with 88px padding.

## Elevation & Depth

Depth is physical: paper and hardware cast long, soft, downward shadows onto the lobby wall as if lit from above; the lobby itself is flat. Shadows are large negative-spread drops (the object floats a few millimetres off the wall), never glows and never hard offsets. Paper objects add a slight rotation (-1.2deg to 0.8deg) to read as placed, not printed.

### Shadow Vocabulary
- **Framed photo** (`0 40px 80px -40px rgba(0,0,0,.85)`): hero door photo, amenities photo, registration card.
- **Card stock** (`0 30px 60px -30px rgba(0,0,0,.8), 0 2px 4px rgba(0,0,0,.2)`): turndown card, check-in slip.
- **Station door** (`0 30px 50px -36px rgba(0,0,0,.9), inset 0 0 0 1px rgba(0,0,0,.06)`).
- **Hung card** (`filter: drop-shadow(0 22px 26px rgba(0,0,0,.45))`): the die-cut door hanger; drop-shadow so the punched hole casts correctly. Mini signs use `drop-shadow(0 6px 6px rgba(0,0,0,.3))`.
- **Push plate** (`0 8px 18px -10px rgba(0,0,0,.7)`, hover `0 12px 22px -10px rgba(0,0,0,.75)`, pressed `0 2px 6px -4px rgba(0,0,0,.6)`): brass buttons only.

### Named Rules
**The Lit-From-Above Rule.** Every shadow falls straight down with a negative spread. No sideways offsets, no coloured glows.

## Shapes

Hotel objects are near-square: card stock at 3px, brass plates and station doors at 4px, photographs at 6px. Round shapes are reserved for things that are round in the world: pill chips and the Menu/flip controls (999px), knobs and key-tag rings (circles). Two silhouettes are signature: the key-tag fob (`999px 6px 6px 999px`, round end toward the tether) and the door hanger (`18px 18px 10px 10px` with a mask-punched circular hole near the top). Holes are real cut-outs via CSS masks, not drawn circles. Inset 1px keylines 10px inside paper and doors give the engraved-border finish.

## Components

### Buttons
Flat brass push plates: solid fill, no gradient, square-ish corners.
- **Shape:** gently squared (4px), min-height 48px (42px in the header).
- **Brass (primary):** brass fill, night-lobby text, uppercase label type, push-plate shadow. Hover: polished brass and a deeper shadow.
- **Ghost:** transparent with a brass hairline (`rule`); hover darkens the border to full brass with a 10% brass wash. Used for the secondary Call action beside Reserve.
- **Ink:** lobby-green fill on linen surfaces (the registration card submit); hover lobby shade.
- **Press:** all buttons sink 2px and scale to .985 on `:active`, shadow collapses. Focus is the global 2px polished-brass outline at 3px offset.

### Chips
- **Fact chip:** pill, 12% brass wash, polished-brass uppercase label. Static facts only, never interactive.

### Cards / Containers (linen card stock)
- **Corner Style:** 3px.
- **Background:** linen to linen-2 gradient, ink text, aged-brass crest at top.
- **Border:** 1px inset keyline in aged brass at ~40–45%, 10px inside the edge.
- **Shadow Strategy:** card-stock shadow, slight rotation.
- **Internal Padding:** `clamp(26–28px, 4vw, 48–56px)`.
- **Variants:** turndown card (bulleted amenity list with aged-brass line icons, italic brass-ink sign-off), check-in slip "Before we arrive" (dashed rule under the header, checkbox squares with ink checkmarks, numbered requirement rows), registration card (the form).

### Inputs / Fields
- **Style:** translucent white (55%) on linen, no box border, 1.5px ink bottom rule at 35%, 3px top corners only (a filled-in form line, not a box).
- **Focus:** background goes solid white, bottom rule becomes lobby green with a 1.5px underline shadow.
- **Error:** bottom rule oxblood, field wash `#fbeeee`, oxblood message below. Labels are uppercase label type in ink-dim; required asterisk in oxblood.

### Navigation
Key-tag fobs on a tether. Each item is a pill-ended tag (`999px 6px 6px 999px`) with a 10% brass wash, a night-lobby hole ringed in 1.5px brass near the round end, and a short brass tether line running off its left edge. Label type in text-dim. Hover: text brightens, wash deepens to 20%, and the tag tilts -3deg from its tether point. Below 1040px the tags stack left-aligned in a night-lobby drawer opened by an outlined pill Menu button; the header keeps the crest + Gilda wordmark lockup. Because the header's brass Book button hides below 1040px, the drawer ends with a brass-rule divider and a full-width pair: brass "Book your date" plate and a ghost call button with the primary number. The drawer closes on link tap, Escape (focus returns to Menu), or a tap outside the header.

### Door Hanger (signature)
A linen die-cut card hung over the hero photo's top-left corner, with a mask-punched hole and a short hanging string. Front: crest, VACANT in plate type, a location line, hairline, short line of copy. Back: oxblood gradient, RESERVED. A pill "Flip the sign" control rotates it 180deg on Y over .9s; it sways once on load (5s, then rests). Stacks above the photo on small phones.

### Station Doors (signature)
Three near-square doors in a row on a night-lobby band, each: linen gradient panel with an inset keyline, a lobby-green restroom sign, a brass "No. n" plate in plate type, and a mini door hanger hung on a brass radial-gradient knob. Hover, focus or tap flips the mini sign from VACANT (lobby) to OCCUPIED (oxblood). A brass hairline "step" runs under the row, followed by a ruled spec strip (uppercase label terms, Gilda values).

### FAQ (front desk)
Hairline-ruled `details` rows; questions in title type; a 28px circular brass-hairline toggle with a polished-brass plus that rotates 45deg when open.

## Do's and Don'ts

### Do:
- **Do** put any new content that a guest must act on inside a linen card-stock object (gradient, 10px inset keyline, card-stock shadow).
- **Do** keep brass for hardware: buttons, numbered plates, rings, tethers, knobs, hairlines and icon strokes.
- **Do** frame photographs at 6px with the framed-photo shadow and a short caption in text-dim; pair them with an object, not with centered overlay copy.
- **Do** set phone numbers and measurements with tabular lining numerals and show both phone lines wherever one appears in a contact block.
- **Do** use the shared easing `cubic-bezier(.16,1,.3,1)` and honour `prefers-reduced-motion` (all animation and transitions off).
- **Do** alternate lobby-wall and night-lobby bands, separated by brass hairlines at roughly 20%.

### Don't:
- **Don't** build a dark full-bleed photo hero with centered copy and a row of gold icon columns; that is the template this world exists to refuse.
- **Don't** use oxblood for emphasis, decoration or a third accent; it is occupied, reserved, required or error only.
- **Don't** set headings or body in Marcellus SC, or bold the Gilda display face.
- **Don't** add gradients, bevels or glossy highlights to the brass buttons; they are flat plates.
- **Don't** cast sideways, hard-offset or coloured shadows.
- **Don't** draw holes on hangers or tags as filled circles on top of the shape; punch them with a mask or ring them like the key tag.
