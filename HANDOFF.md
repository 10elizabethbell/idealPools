# Ideal Pools, LLC — handoff at ~60%

**Live:** https://10elizabethbell.github.io/idealPools/ · **Repo:** https://github.com/10elizabethbell/idealPools · **Built:** 2026-10-19 from Muse brief (run 2026-10-19, Ocean County group pool-closing post)

## What's built
- One phone-first page (`index.html`, ~48KB, no frameworks or tracking) plus `img/` (logo in 3 sizes, favicon, home-screen icon, 1200x630 link preview).
- **World:** the pool at closing time. Logo navy ground, sun-yellow buttons, frost-white light bands, royal-blue cues.
- **Signature element:** the hero's pool band. It has clear water with moving light patterns and real ripples, a stone edge with a waterline tile strip, and autumn leaves floating on it. A skimmer net glides over and scoops the leaves by itself. A finger or mouse takes the net over in every direction, and leaves fall back in after a few seconds. Moving waterlines divide every section.
- **Sections:**
  - Header: logo, name, and (848) 480-3729 top-right.
  - Hero: "Your pool, safe all winter.", Check availability, Message us on Facebook (opens Messenger via m.me).
  - "We service all types of pools.": pool types and 9 service rows. Each row jumps to the form with that service ticked.
  - About: owner-voice promise, the full logo badge on phones, a "Visit our Facebook to see more." button.
  - Booking takes a minute (3 steps).
  - Check availability form.
  - Footer: name, phone, Facebook.
- **Contact:** the form composes a pre-written text to (848) 480-3729. If messages don't open, a panel offers Copy message and Send it on Messenger, and the form has a call link. Validation is inline, and screen readers announce it.
- **Checked:** Chromium and WebKit at 360, 390, 430 and 1440. No sideways scroll, tap targets 44px+, the primary button on the first screen, touch and mouse sweeps move the net and scoop leaves, motion frames differ, the SMS body decodes correctly, no script errors.
- **Impeccable:** finish review plus every mode except live and onboard. Fixes applied. The detector's font, padding and type-scale notes are waived in `.impeccable/config.json` with reasons.

## Assumptions I made
- **Services come from the logo badge, not just the brief.** The badge lists opening, closing, cleaning, liner replacement, equipment repairs, acid washes, leak detection and deck coatings, plus "We specialize in building above ground pools". I listed all of them, plus "Above-ground pool builds".
- **Voice is "we"** (an LLC; the caption says "Message us").
- **Colors** are sampled from the logo: navy band, royal and sky blue, the sun's yellow.
- **The headline** "Your pool, safe all winter." comes from the flyer's "Keep Your Pool Safe This Winter!" and "Peace of mind all winter long".
- **About copy is mine, in their voice:** "We close your pool like we'll be the ones opening it in spring, because we'd like to be." The facts behind it are theirs: new in 2026, 10+ years' experience, above-ground specialty.
- **Not used:** "Reliable and affordable" (it reads like any company's line) and the flyer image (a promo graphic, not work).

## Placeholders and gaps
- **No real job photos anywhere** (Facebook has only promo graphics). There's no photo/proof section; the logo badge and Facebook link stand in. This is the first thing to add.
- **No service area** (the brief says don't infer one), so there's no area section. The form asks for the town.
- **No hours, email, owner name, license/insurance, reviews or prices** on the page.
- **Header logo:** the badge is detailed and unreadable at 52px. The favicon and home-screen icon use a crop of its sun/wave/pool art.
- **No concept-roll seed key** in the direction contract. This was a code-led, unattended build, so the roll didn't run.

## Questions for the owner
1. **Does (848) 480-3729 take texts?** The form's main button sends a text. If it's a landline, switch the submit to copy the message and open Messenger (`https://m.me/61572061220492`).
2. Which towns do you cover? This would add a service-area line.
3. Photos of real closings, openings, liner jobs or above-ground builds, and any before/afters.
4. Your first name, for the About section ("I'm ___, and…").
5. Hours, and whether you're licensed and insured.
6. Any customer reviews we can quote word for word.
7. An email for the footer, if you want one.
8. Which services matter most after closing season? The order could change by season (openings first in spring).

## Ideas not built (yours to pick)
- **Runner-up world:** frost forming on a winter cover that your finger wipes clear. Stronger for "safe all winter", but less fun to play with than skimming.
- **Seasonal swap:**
  - Winter: leaves become snowflakes, and a cover slowly eases across part of the pool.
  - Spring: the hero says "Open clear this spring."
- The waterline tile strip could edge the form section, to carry the pool world below the hero.
- A tiny reward when the visitor clears every leaf: the net "taps" and a "Clean!" splash.
- Before/after sliders once real photos exist (green pool → clear).
- A booking page (`book.html`), only if the one-page form proves too long.
- A desktop hole remains: the left column under "We service all types of pools." Proof photos could go there.

## Not verified
- Real-device touch on an iPhone and an Android phone, inside Facebook's in-app browser. That includes dragging the net up and down without the page scrolling or pull-to-refresh.
- That the `sms:` link opens Messages with the body filled on iOS and Android.
- That `m.me/61572061220492` opens a Messenger thread inside the Facebook app. It resolves to a thread over the web; I didn't test it in the app.
- Frame rate on older phones. Headless frame time was about 8ms (Chromium) and 16ms (WebKit).
