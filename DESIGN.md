---
name: Ideal Pools, LLC
description: Calm paper and navy bands with the logo's sun as the one warm fill, for a pool crew that closes pools late in the season.
colors:
  sun: "#ffc83d"
  sun-hover: "#ffd76b"
  sun-ink: "#8a5a00"
  navy: "#134a8e"
  deep: "#0b2a4a"
  ink: "#0b2a4a"
  focus: "#1a63c9"
  paper: "#f4f6fb"
  card: "#ffffff"
  field: "#e6ecf5"
  body: "#28394d"
  soft: "#4a5a6c"
  on-dark: "#f4f7fb"
  on-dark-soft: "#c9d8ec"
  error: "#b3261e"
typography:
  display:
    fontFamily: "\"Cal Sans\", \"Avenir Next\", \"Segoe UI\", system-ui, sans-serif"
    fontSize: "clamp(42px, 12vw, 80px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "\"Cal Sans\", \"Avenir Next\", \"Segoe UI\", system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  callout:
    fontFamily: "\"Cal Sans\", \"Avenir Next\", \"Segoe UI\", system-ui, sans-serif"
    fontSize: "clamp(30px, 9vw, 52px)"
    fontWeight: 400
    lineHeight: 1
  title:
    fontFamily: "\"Cal Sans\", \"Avenir Next\", \"Segoe UI\", system-ui, sans-serif"
    fontSize: "clamp(19px, 5.2vw, 22px)"
    fontWeight: 400
    lineHeight: 1.2
  action:
    fontFamily: "\"Cal Sans\", \"Avenir Next\", \"Segoe UI\", system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.7
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 500
    lineHeight: 1
    letterSpacing: "0.02em"
  scale:
    xxs: "11px"
    xs: "14px"
    sm: "15px"
    base: "16px"
    md: "17px"
    lg: "18px"
    lg-plus: "19px"
    xl: "20px"
    xl-plus: "21px"
    xxl: "22px"
    brand: "24px"
    h-min: "30px"
    h1-min: "42px"
    h-max: "48px"
    callout-max: "52px"
    h1-max: "80px"
rounded:
  field: "10px"
  focus: "6px"
  panel: "16px"
  feature: "20px"
  card: "24px"
  pill: "999px"
spacing:
  chip-gap: "10px"
  field-gap: "8px"
  head-gap: "16px"
  gutter: "20px"
  gutter-desktop: "40px"
  form-gap: "22px"
  section: "64px"
  section-desktop: "96px"
components:
  button-primary:
    backgroundColor: "{colors.sun}"
    textColor: "{colors.ink}"
    typography: "{typography.action}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.sun-hover}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.action}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.action}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  eyebrow:
    backgroundColor: "rgba(11,42,74,.06)"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "9px 14px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card}"
  input:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  form-card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  ready-panel:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.panel}"
    padding: "18px"
  facebook-card:
    backgroundColor: "{colors.card}"
    textColor: "{colors.ink}"
    typography: "{typography.title}"
    rounded: "{rounded.feature}"
    padding: "14px 16px 14px 22px"
    height: "72px"
  service-row:
    textColor: "{colors.on-dark}"
    typography: "{typography.title}"
    height: "64px"
  text-circle:
    backgroundColor: "{colors.sun}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "60px"
---

# Design System: Ideal Pools, LLC

## Overview

**Creative North Star: "The Calm Band"**

The page is a stack of full-bleed bands that alternate light and dark, so every new section is obvious on a phone without a single divider: paper header, navy hero, paper About, navy services, paper booking form, navy close, deep-navy footer. All the colour comes from the logo badge. Its royal blue, deepened, makes the main dark band. Its navy band makes the deepest one, with a faint diagonal-line texture. Its sun is the one warm note, and it only ever appears as a fill.

This is the pitch-site calm band house style (after lpmr.co.uk) applied to Ideal Pools. Shapes are soft and borderless: a 24px card, full pills, tinted fields with no border. One display webfont (Cal Sans) carries every heading and action, and the system stack carries running text at 16/1.7. Motion is limited to three moments: the hero H1 bounces in letter by letter, content below the first screen fades up 12px once, and a floating sun-yellow text circle slides in after the hero. The hero is a plain navy band because no real job photos exist yet. A real photo under a navy overlay replaces it once one fits the band at both 390px and 1440px.

There are no shadows apart from the floating circle, no gradients apart from the line texture, and no imagery apart from the logo badge.

**Key Characteristics:**
- Full-bleed paper and navy bands alternate down the page; the section boundary is the colour change.
- The sun yellow is a fill (buttons, the text circle, the eyebrow dot, a hovered arrow). Any text on it is ink.
- One display face (Cal Sans, weight 400) for headings, buttons, labels and phone numbers; system sans for everything else.
- Soft, borderless shapes: 24px cards, full pills, 10px tinted fields.
- Flat throughout. Depth comes from tone, and the floating circle is the only thing with a shadow.
- Three motion moments, all switched off under reduced motion.

## Colors

Cool off-white paper, two logo navies, and one warm sun used as a fill.

### Primary
- **Sun Yellow** (sun): the logo's sun. Fills the primary pill button, the floating text circle, the eyebrow dot, the separators in the pool-type list, the text-selection highlight, and an arrow circle on hover or focus. On dark bands it also colours the accent phrase in a heading, the phone glyph and link hover. Any text on a sun fill is Ink.
- **Sun Hover** (sun-hover): the lighter sun used for the primary button's hover fill and border. Only for hover.
- **Sun Ink** (sun-ink): the sun darkened to 5.6:1 on paper, for when the accent has to be text or a glyph on a light ground: the accent phrase in a paper-band heading, the header phone icon, the header phone hover.

### Secondary
- **Logo Royal Navy** (navy): the logo's royal blue, deepened. The ground for the hero and the services and close bands. Also the Facebook glyph and the input caret.
- **Band Navy** (deep): the logo's navy band. The footer ground, always under the diagonal-line texture.
- **Focus Royal** (focus): a brighter logo blue, used for the outline on hover and focus of form controls and for focus rings on light bands. It is kept distinct from the yellow fill so that focus never looks like selection.

### Neutral
- **Ink** (ink): headings on light bands, text on sun fills, the selected-chip fill, the outline button. It has the same value as Band Navy but a different role.
- **Paper** (paper): the page ground, the header, the light bands and the ready panel inside the form.
- **Card White** (card): the booking form card, the Facebook card and the message preview. Also pure white text: the hero H1 and selected chip labels.
- **Field Tint** (field): the fill for inputs and unselected chips on the white form card. It exists because a paper fill on white measured about 1.08:1.
- **Body Slate** (body): running text on light bands.
- **Soft Slate** (soft): ledes, the "(optional)" tag, placeholders, the note under the submit button, the wordmark's "LLC".
- **On-Dark** (on-dark): headings, service rows and links on navy bands.
- **On-Dark Soft** (on-dark-soft): running text, ledes and the promise line on navy bands.
- **Error Red** (error): inline error sentences, and the input border while a field is invalid.

Translucent tints are derived from these colours, not added as tokens: ink at 6-7% (eyebrow and arrow-circle fills on paper, the outline button's hover) and white at 10-14% (eyebrow, arrow circle and hairline row dividers on navy, the ghost button's hover). On-Dark at 70% is the ghost button's border.

### Named Rules
**The Sun Is A Fill Rule.** The sun yellow fills; it does not write on light. Text on a sun fill is Ink. When the accent has to be text on paper, it is Sun Ink. White on sun and sun on paper both fail contrast at about 2.2:1.

**The Accent Phrase Rule.** In a heading, only the last phrase takes the accent colour ("safe all winter.", "all types of pools."): Sun on navy, Sun Ink on paper. At most one accent phrase per heading.

## Typography

**Display Font:** Cal Sans (with "Avenir Next", "Segoe UI", system-ui, sans-serif), from Google Fonts with preconnect and `display=swap`
**Body Font:** the system stack (-apple-system, BlinkMacSystemFont, "Segoe UI", "Helvetica Neue", Arial, sans-serif)

**Character:** Cal Sans at weight 400 is rounded and friendly without looking childish, and it sets every heading, button, form label, service row and phone number. The system body face stays out of its way.

### Hierarchy
- **Display** (display): the hero H1 only. White on navy, at most 11ch wide, letter-spacing -0.005em.
- **Headline** (headline): section H2s, line-height 1.08, balanced wrapping.
- **Callout** (callout): the big tap-to-call number in the close band.
- **Title** (title): service rows on navy, and the Facebook card (18-20px).
- **Action** (action): button labels, plus the header phone (17px, 20px on desktop), form labels and legends (17px), and the wordmark (21px, 24px on desktop).
- **Lede** (lede): the intro paragraph under an H2 (38ch, 46ch in the About band on desktop). The hero promise line is the same voice at 17-20px and line-height 1.5, 30ch on phones.
- **Body** (body): running text, inputs and chips. Never below 16px on a field, so iOS doesn't zoom.
- **Label** (label): the eyebrow pill text. Smaller steps are 15px for error sentences, the after-submit note and the message preview, and 14px for the "(optional)" tag.
- **Wordmark small**: the "LLC" under the name, 11px, weight 600, tracked 0.08em, uppercase. This is the only uppercase on the page.

### Named Rules
**The One Display Face Rule.** Cal Sans is the only webfont and appears only at weight 400. Hierarchy comes from size and colour, never from a bold display weight or a second display family.

**The Display Talks Rule.** Anything the user reads as a call or a thing to tap (buttons, rows, labels, phone numbers) is set in Cal Sans. Explanations and fine print are set in the system face.

## Layout

The page is a single centred column, 1160px max, with a 20px phone gutter that widens to 40px from 760px. Bands are full-bleed; their content sits in the column. Vertical rhythm is 64px of section padding on phones and 96px from 760px. The hero has its own padding: 56/68px on phones, 96/112px on desktop.

- **Phones first.** Everything stacks in one column. The hero's two buttons stack full width, and the form's submit button is always full width.
- **From 760px:** the hero buttons sit side by side at 240px minimum, and the ready-panel buttons line up in a row.
- **From 1024px:** the hero becomes text plus the 360px logo badge on the right. The services and booking bands become two columns (head 1fr against 1.6fr / 1.4fr), and their headings stick at 40px from the top while the rows or the form scroll. Service rows become two columns with a 40px gap. The close band puts the name on the left and the big number bottom-right.
- **Internal gaps:** heading groups 16px, the form 22px between fields, 8px from a label to its field, 10px between chips.
- **Below 380px:** chip side padding drops from 18px to 14px so short chips still pair up on a row.

**The Band Is The Divider Rule.** Sections are separated by a change of band colour, never by rules, borders or cards floating on one shared ground. The only hairlines are the dividers between service rows on navy (white at 14%).

## Elevation & Depth

The system is flat. Depth comes from tone: a white card on paper, a tinted field on a white card, a paper panel inside the white form. There is one shadow, and it belongs to the one element that floats above the scroll.

### Shadow Vocabulary
- **Float lift** (`box-shadow: 0 10px 28px rgba(6,22,42,.3)`): the floating text circle only. It is a soft, navy-tinted ambient lift so the yellow circle separates from whatever band is behind it.

### Named Rules
**The One Floating Thing Rule.** Only the fixed text circle casts a shadow. Cards, buttons, the header and hover states stay flat. Hover handlers on the Facebook card and the service rows explicitly cancel any shadow.

**The Faint Lines Rule.** The diagonal-line texture (135deg, transparent for 22px then white at 3.5% for 1px) only appears on the dark bands: the hero and the footer. It stays at about 4% white or fainter so it never reads as lines through text.

## Shapes

Soft and borderless. Containers have a generous radius, every control is a pill or a soft tinted rectangle, and circles are reserved for the logo, the arrows and the floating button.

- **Card** (card radius): the booking form card.
- **Feature** (feature radius): the Facebook card in About. Slightly tighter than the form card because it is a single-row link.
- **Panel** (panel radius): the "Your message is ready" panel nested inside the form card. It steps down from the card radius so the nesting reads.
- **Field** (field radius): text inputs, the textarea and the message preview.
- **Focus** (focus radius): the corner of the global focus outline on links and text.
- **Pill** (pill radius): buttons, chips and the eyebrow.
- **Circles** (50%): the logo badge (also clipped to a 48.5% circle to trim its edge), 44px arrow circles and the 60px floating text circle.

Borders exist only as states: 2px transparent borders on buttons, fields and chips, coloured in on hover, focus or error. The outline and ghost buttons are the only components with a resting border.

## Components

### Buttons
Full pills, 56px tall, set in Cal Sans. They press in slightly (scale .98) when tapped.
- **Primary (sun):** a Sun Yellow fill with an Ink label. The hero's "Check availability" and the form's "Text this to Ideal Pools" (full width, with a chat glyph). On hover it takes the Sun Hover fill. Inside the form it also gets a 3px Focus Royal outline on hover and focus, offset by 3px.
- **Ghost (on navy):** transparent, with an On-Dark label and a 2px On-Dark border at 70%. On hover the border turns full white over a 10% white fill. Used for "Message us on Facebook" in the hero.
- **Line (on light):** transparent with an Ink label and border, and a 6% ink fill on hover. Used for the ready panel's "Copy message" and "Send it on Messenger".
- **Limit:** at most two buttons in the hero (one primary, one ghost). There is no Call button; the number lives in the header.

### Chips
- **Style:** 48px pills with a Field Tint fill, Ink text in the 16px system face, and a 2px transparent border.
- **State:** hovering colours the border Focus Royal. Selected chips take an Ink fill with white text. Keyboard focus is a 3px Focus Royal outline at a 2px offset, because a border on the ink fill measured only about 1.6:1. The same chip handles multi-select (services) and single-select (pool type, timing).

### Cards / Containers
- **Form card:** Card White, card radius, with padding that scales from 20px to 32px. There is no shadow and no border.
- **Ready panel:** Paper inside the white card, panel radius, 18px padding. It holds the composed message in a white, field-radius preview block (15px/1.5) and two line buttons.
- **Facebook card:** a Card White row 72px tall with feature radius, a Logo Royal Navy Facebook glyph, a Cal Sans label and an arrow circle on the right. Only the arrow changes on hover and focus.

### Inputs / Fields
- **Style:** a Field Tint fill with field radius, no visible border (2px transparent), 52px tall, 16px text in Ink, Soft Slate placeholders. The textarea is 110px minimum and resizes vertically.
- **Hover / Focus:** the border turns Focus Royal. There is no glow.
- **Error:** the border turns Error Red and stays red while focused (the rule is declared later and is more specific). A plain-sentence error appears in 15px Error Red under the field ("Add your name so we know who's asking.").
- **Labels:** Cal Sans 17px in Ink, tied to fields with `for`. Optional fields carry a soft "(optional)" tag.

### Navigation
- **Header:** a slim paper bar, 68px tall (80px on desktop). The round logo and the Cal Sans wordmark (with the small "LLC" beneath) sit on the left. The tap-to-call number sits top-right with a Sun Ink phone glyph and turns Sun Ink on hover. There is no menu.
- **Footer:** Band Navy with the line texture. It holds the name and number, a Facebook link (44px tall, On-Dark, turning Sun on hover) and the copyright. The bottom padding clears the floating circle.

### Service Rows (signature)
Each row on the navy band is a link: a Cal Sans service name with a 44px arrow circle on the right, at least 64px tall, separated by 14% white hairlines. They are one column on phones and two on desktop. Only the arrow changes: its circle goes from 10% white to a Sun Yellow fill with Ink arrow on hover, and on keyboard focus it also gets a Sun outline. Tapping a row pre-selects the matching chip in the booking form.

### Eyebrow Pill (owner-mandated exception)
A quiet 14px label pill above three headings only: the hero ("Last-minute pool closings"), services and the booking form. It has an ink fill at 6% (white at 12% on navy), a 7px sun dot before the text, no arrow, no hover state and no shadow. It is marked up as a `<p>`, never as a heading. Ellie chose these pills for the calm house style on 2026-10-19. Impeccable's craft floor flags eyebrows as an anti-pattern, so treat this as a recorded exception, not a pattern to extend: do not add eyebrows to further headings, and do not give one a strong sun fill.

### Floating Text Circle (signature)
A 60px Sun Yellow circle fixed 16px from the bottom-right corner (plus safe area), with an Ink chat glyph and the Float lift shadow. It opens `sms:` with a pre-filled greeting. It slides up from 120px below the screen (.35s, cubic-bezier(.2,.8,.2,1)) once the hero has scrolled away, and hides again while the booking form is on screen. While hidden it is `tabIndex=-1` and `aria-hidden`. It is one circle, never a bottom bar, and it does not exist without JS or when `CONFIG.FLOAT` is false.

### Motion
- **Hero H1 bounce-in:** the hero H1 only. JS splits it into letters inside nowrap word wrappers. Each letter goes from opacity 0 at translateX(50px) to rest over 1s on cubic-bezier(.34,1.56,.64,1), 20ms apart. When the last letter finishes, the original markup is restored. It is skipped without JS and under reduced motion.
- **Fade-up:** blocks marked to rise move up 12px and fade in over .4s ease-out, and only if they start below the first screen. Everything is visible at rest, without JS, and under reduced motion.
- **State transitions:** colour changes take .2s on buttons and arrows and .15s on fields and chips; a press scales to .98 over .12s.

## Do's and Don'ts

### Do:
- **Do** alternate full-bleed paper and navy bands and let the colour change separate sections.
- **Do** use Sun Yellow only as a fill with Ink on it; use Sun Ink when the accent has to be text on paper.
- **Do** set headings, buttons, labels, rows and phone numbers in Cal Sans at weight 400, and running text in the system stack at 16/1.7.
- **Do** give inputs and chips the Field Tint fill on the white card, and outline them in Focus Royal on hover and focus.
- **Do** keep tap targets at 44px or more (buttons 56px, chips 48px, fields 52px, rows 64px).
- **Do** keep the hero to an eyebrow, the H1, one promise line and at most two buttons, with the phone number in the header.
- **Do** keep all motion off under `prefers-reduced-motion`, with everything visible at rest.

### Don't:
- **Don't** put white or paper text on the sun, or sun text on paper.
- **Don't** add shadows to cards, buttons or the header; the floating text circle is the only lifted element.
- **Don't** letter-animate any heading other than the hero H1, and don't add a second motion style beyond the one 12px fade-up.
- **Don't** add a second webfont or a bold Cal Sans.
- **Don't** add eyebrow pills beyond the three that exist, or style one like a button.
- **Don't** let the line texture go above about 4% white or onto a light band.
- **Don't** turn the floating circle into a bottom bar, or show it while the booking form is on screen.
