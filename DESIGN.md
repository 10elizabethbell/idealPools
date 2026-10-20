---
name: Ideal Pools, LLC
description: Last-minute pool closings, told from the pool edge at closing time.
colors:
  sun: "#ffc83d"
  sun-hover: "#ffd76b"
  royal: "#1a63c9"
  pool: "#1aa0dc"
  sky: "#7fd0f5"
  navy: "#0b2a4a"
  navy-2: "#0e355e"
  navy-deep: "#081f38"
  frost: "#eef5fb"
  frost-2: "#dcebf6"
  ink: "#0d2441"
  ink-soft: "#3c5672"
  on-navy: "#ffffff"
  on-navy-soft: "#c4d9ee"
  error-line: "#ff9b8a"
  error-text: "#ffb4a6"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2.6rem, 12.4vw, 5.6rem)"
    fontWeight: 900
    lineHeight: 1.02
    letterSpacing: "-0.01em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(1.9rem, 8vw, 3.2rem)"
    fontWeight: 900
    lineHeight: 1.02
    letterSpacing: "-0.01em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "20px"
    fontWeight: 700
    lineHeight: 1.2
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 800
    lineHeight: 1.25
  small:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "15px"
    fontWeight: 600
    lineHeight: 1.55
rounded:
  field: "12px"
  card: "14px"
  pill: "999px"
  circle: "50%"
spacing:
  gutter-phone: "16px"
  gutter-desk: "40px"
  section-phone: "56px 0 72px"
  section-desk: "88px 0 104px"
  column-gap: "64px"
components:
  button-sun:
    backgroundColor: "{colors.sun}"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 24px"
    height: "56px"
  button-sun-hover:
    backgroundColor: "{colors.sun-hover}"
    textColor: "{colors.ink}"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.on-navy}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 24px"
    height: "56px"
  button-line-hover:
    textColor: "{colors.sun}"
  chip:
    backgroundColor: "transparent"
    textColor: "{colors.on-navy}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "46px"
  chip-selected:
    backgroundColor: "{colors.sky}"
    textColor: "{colors.ink}"
  input:
    backgroundColor: "#ffffff"
    textColor: "{colors.ink}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  service-row:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.title}"
    height: "60px"
  service-row-arrow:
    backgroundColor: "{colors.frost-2}"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "40px"
  service-row-arrow-hover:
    backgroundColor: "{colors.royal}"
    textColor: "#ffffff"
  step-number:
    backgroundColor: "{colors.royal}"
    textColor: "#ffffff"
    rounded: "{rounded.circle}"
    size: "44px"
  facebook-card:
    backgroundColor: "#1877f2"
    textColor: "#ffffff"
    rounded: "{rounded.card}"
    padding: "18px 20px"
---

# Design System: Ideal Pools, LLC

## Overview

**Creative North Star: "The Pool at Closing Time"**

The page is the pool on the last warm weekend: logo-navy ground, a real pool edge (stone coping, blue waterline tile), clear water with moving light, autumn leaves on the surface, and a skimmer net working them off. Every section boundary is a moving waterline, so the whole scroll reads as going down through water bands. The palette comes straight from the logo badge (navy band, royal and sky blue, yellow sun, white lettering); the frost-white light bands come from the closing-season flyer.

The voice is the type, not the face: heavy (900) uppercase headlines on the system sans stack, sentence-case body and labels. The system stack is deliberate house style for this build (fast in Facebook's in-app browser, no font requests). Density is phone-first and generous: 56px buttons, 17px body, one long single column that splits into two-column grids at 1024px.

This build was code-led: no image generation and no concept-roll seed key exists for it. The direction contract lives as the HTML comment at the top of `<body>` in `index.html`; this file records what shipped. Future edits are also bound by the pitch-site finishing rules (`~/.claude/skills/pitch-site/references/finishing-rules.md`); the ones that touch this system are cited inline below.

**Key Characteristics:**
- Logo-derived palette: navy grounds, sun-yellow primary action, royal/sky for cues and form focus.
- Heavy uppercase display, sentence-case everything else, system sans.
- One living hero (canvas pool) plus moving SVG waterline seams; nothing else animates beyond control feedback.
- Pill buttons and chips, circle markers, softly rounded cards; flat surfaces otherwise.
- Contact flows by text message (SMS composed from the form) with Messenger as fallback.

## Colors

A logo palette on two grounds: deep navy bands and frost-white bands alternate, with one warm accent.

### Primary
- **Sun Yellow** (`sun`): the only fill for primary actions ("Check availability", "Text this to Ideal Pools"), the phone icon in the header, text selection, the global focus ring, and hover color for header/footer links. `sun-hover` is its lighter hover step.

### Secondary
- **Royal Blue** (`royal`): cues on light grounds. Service-row arrow on hover, step number discs, the dot separators in the pool-types line.
- **Sky Blue** (`sky`): the form's single interaction accent on navy. Input/chip hover and focus outlines, the selected-chip fill, the chip splash ring, light-band seam lines.

### Tertiary
- **Pool Blue** (`pool`): seam line color on navy-ground sections and the footer. Water itself is drawn procedurally in the canvas, not from tokens.

### Neutral
- **Logo Navy** (`navy`): page ground, hero, About band.
- **Booking Navy** (`navy-2`): the booking section only, one step lighter so the form reads as its own place.
- **Deep Navy** (`navy-deep`): footer.
- **Frost** (`frost`) and **Frost Deep** (`frost-2`): light section ground, and the resting arrow circle on it.
- **Ink** (`ink`) and **Ink Soft** (`ink-soft`): headings/body and secondary copy on frost. Row dividers are ink at 14% alpha.
- **White** (`on-navy`) and **Mist** (`on-navy-soft`): headings and secondary copy on navy.
- **Error coral** (`error-line`, `error-text`): invalid field border and message on navy.

### Named Rules
**The Accent-On-Hover Rule.** Accents appear on interaction, not at rest: the service arrow is neutral frost until hovered, links turn sun only on hover (finishing rules: "Accent color on hover, not by default").

**The One Form Accent Rule.** Inside the form every control outlines in sky on hover and focus. Never sun there; sun is already the button fill.

## Typography

**Display Font:** system sans stack (-apple-system, Segoe UI, Roboto, Helvetica Neue, Arial)
**Body Font:** same stack

**Character:** One family, two registers. Black-weight uppercase for headlines and the wordmark gives the flyer's urgency; plain sentence-case body keeps it a neighbour talking.

### Hierarchy
- **Display** (900, clamp 2.6rem to 5.6rem, 1.02, uppercase, max 11ch, balanced): hero headline only.
- **Headline** (900, clamp 1.9rem to 3.2rem, 1.02, uppercase, balanced): one per section, short and ending with a period.
- **Title** (700, 20px, 1.2, sentence case): service rows (22px at desktop) and step headings (which override the uppercase h3 default).
- **Body** (400, 17px, 1.55): paragraphs, max 60ch in About; hero promise 17-20px in mist, max 34ch.
- **Label** (800, 17px): buttons, form labels, header phone number (tabular numerals, 20px at desktop).
- **Small** (600-700, 15px): chips, form notes, errors, footer.

### Named Rules
**The Shout-Only-Headlines Rule.** Uppercase is for h1/h2 and the wordmark. Body, labels, chips, rows and step titles stay sentence case.

## Layout

Single long page, phone-first: header, hero with pool band, Services (frost), About (navy), How it works (frost), Booking (navy-2), footer (navy-deep). Content sits in a 1180px max container with a 16px gutter (40px from 1024px), padded by safe-area insets. Sections pad 56/72px on phones and 88/104px at desktop.

At 640px hero actions go from a stacked grid to a wrapping row (min 230px each). At 1024px sections become asymmetric two-column grids with a 64px gap: Services 5/7 (heading left, rows right), About 7/5 (copy left, Facebook card right, bottom-aligned), Booking 4/8 with a sticky heading and a two-column form (chip groups, town and notes span full). Steps become three columns.

**The Header Number Rule.** The phone number lives top-right in the header as a `tel:` link and is the only number on the first screen; no Call button under the hero title, at most two hero buttons (finishing rules: contact buttons).

## Elevation & Depth

Flat by default; depth comes from alternating navy and frost bands and from the canvas scene's own lighting. Shadows are soft, downward and few.

### Shadow Vocabulary
- **Button lift** (`0 6px 14px -6px rgba(3,14,30,.55)`): sun buttons only.
- **Badge drop** (`0 24px 40px -18px rgba(2,12,28,.75)`): the round logo badge, both placements.
- **Card drop** (`0 14px 30px -16px rgba(0,0,0,.6)`): the Facebook card.

**The Real-Material Rule.** Depth inside the pool is physical: blurred leaf and net shadows that shift with the water slope, shade under the coping. No sheens, films or glints (finishing rules: "Every effect must read as a real thing").

## Shapes

Water-smooth: pills (999px) for every button and chip, full circles for logo marks, arrow discs and step numbers, 12px on inputs, 14px on cards (Facebook card, composed-message panel). Lists use hairline ink dividers rather than boxes. The only non-rounded edges are the seams' organic wave lines and the pool's straight coping, which is a built edge and reads as one.

## Components

### Buttons
- **Shape:** pill, 56px tall, 2px border, label weight.
- **Sun (primary):** sun fill, ink text, button lift; hover lightens to `sun-hover`.
- **Line (secondary):** outlined in white at 70%, white text; hover turns border and text sun. Secondary hero buttons are always outlined, never filled (finishing rules).
- **Press:** scale(.98). Inside the form, buttons also take a 3px sky outline on hover and focus.

### Chips (form choices)
- **Style:** 46px pill, 2px white-35% border, white 15px text on booking navy. Real checkbox/radio inputs, visually hidden.
- **State:** hover/focus border sky; selected fills sky with ink text; a sky ring splashes outward (0.55s) when ticked, including when a service row pre-selects it. Chips are only for choices; never for non-interactive labels or towns (finishing rules).

### Inputs / Fields
- **Style:** white field, 12px radius, 52px min height, 2px transparent border, bold 17px label above; "(optional)" in mist.
- **Focus:** sky border plus 2px sky outline. **Error:** coral border and a 15px coral line under the field naming exactly what to add.

### Service Rows
- **Style:** full-width links, title type, hairline dividers, trailing 40px arrow disc in frost-2.
- **Hover/Focus:** only the arrow changes (royal fill, white arrow, 2px nudge right); the focus ring sits on the arrow. Clicking a row ticks that service's chip and scrolls to the form.

**The Arrow-Only Rule.** A tappable row never gets an outline, border, ring or tint. Only its arrow highlights (finishing rules, quoted from Ellie).

### Booking flow (signature)
Submitting validates, then composes a plain text message (service, pool, when, town, name, phone, notes) and opens `sms:` to the business. A "Your message is ready" panel (white 7% on navy, 14px radius) shows the text with two line buttons: Copy message and Send it on Messenger. The note under the button explains it opens a pre-written text and offers the call. No email anywhere except a footer email if one is ever supplied.

### Logo badge
The round logo badge appears once per layout: on desktop it floats over the hero's pool edge on the right (240-310px, pointer-events off); on phones it sits centered in About above the Facebook card (max 300px). Header and footer carry the small round mark beside the wordmark.

### Facebook card
Facebook-brand-blue card with the f-mark, 20px bold "Visit our Facebook to see more.", trailing arrow. It sits in About where visitors look for proof, and Facebook is repeated in the footer (finishing rules: Facebook).

### Pool hero canvas (signature)
Below the hero copy, a canvas band (250-440px tall): 56px of open air where leaves fall, 16px stone coping with joints and speckle, 13px blue waterline tile, then water rendered from a damped ripple heightfield with sine-interference caustics. 9 leaves on phones, 18 at desktop, three leaf shapes in five autumn colours, each with a soft slope-shifted shadow. A skimmer net (blue frame, mesh, aluminium pole off the bottom right) auto-glides to the nearest leaf until touched; a finger or mouse takes it over in every direction (touch-action none, position read every frame) and it returns to auto 3.5s after the last touch. Leaves scooped by a moving net fade out and fall back in after 3-7s. Tunables live in the `CFG` block. One shared requestAnimationFrame loop drives the canvas and seams, pauses off screen, and under reduced motion draws one still frame (waking briefly on touch).

### Waterline seams
Each section and the footer opens with an SVG wave (34px, 48px at desktop) filled in the section's own ground colour, with a 2.5px line on top: sky over frost bands, pool blue over navy bands. Three summed sines move continuously, phase-offset per seam.

**The Moving Waterline Rule.** Section changes are waterlines, never straight rules or slanted cuts. Seams stay clear of text (finishing rules: nothing runs through text).

## Do's and Don'ts

### Do:
- **Do** use sun for primary fills only, sky for every form hover/focus outline, royal for cues on frost.
- **Do** keep headlines uppercase 900 and short; keep all other text sentence case.
- **Do** give every new section a seam in its own ground colour and alternate navy and frost grounds.
- **Do** keep the hero to one focal point: headline, promise, at most two buttons, the pool band.
- **Do** tune the pool through `CFG`, and keep the net working by itself until touched.
- **Do** keep the phone-first sizes: 56px buttons, 46px chips, 44px minimum tap targets.

### Don't:
- **Don't** highlight a service row; only its arrow changes on hover.
- **Don't** show accents at rest on interactive cues; they arrive on hover.
- **Don't** add a Call button under the hero, a second phone number on the first screen, or a sticky bottom bar.
- **Don't** put towns or non-interactive labels in pills or chips; use plain dot-separated text like the pool-types line.
- **Don't** lay sheens, glints or ruler-straight "nature" lines over the scene; every effect must read as the real thing.
- **Don't** add animation beyond the pool, the seams and control feedback. If this audience is ever confirmed 40+, the older-audience rules apply: draw the pool once as a still and stop the seams.
