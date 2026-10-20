# Ideal Pools, LLC — handoff at ~60%

**Live:** https://10elizabethbell.github.io/idealPools/ · **Repo:** https://github.com/10elizabethbell/idealPools · **Built:** 2026-10-19 from Muse brief (run 2026-10-19, Ocean County group pool-closing post); restyled to the calm band style the same day · **Call Sheet:** site URL set

## What's built
- One phone-first page (`index.html`, ~30KB, no frameworks or tracking; Cal Sans from Google Fonts for headings) plus `img/` (logo in 3 sizes, favicon, home-screen icon, 1200x630 link preview).
- **Calm band style:** off-white paper and navy bands, coloured from the logo. The bands are royal blue deepened to #134a8e and the logo's navy band #0b2a4a with the faint line texture. The logo's sun yellow is the one accent, used as a fill with navy text on it.
- **Hero:** a plain textured navy band (no photo; see gaps). It has the eyebrow "Last-minute pool closings", "Your pool, *safe all winter.*" bouncing in letter by letter, "It's not too late. Message us today to ask about availability." and two buttons: Check availability (filled) and Message us on Facebook (outlined, opens Messenger via m.me). On desktop the logo badge sits on the right.
- **Sections:**
  - Header: logo, name, and (848) 480-3729 top-right.
  - Hero.
  - About on paper: "New company. Ten years of pools.", the owner-voice promise, the logo badge on phones, and a "Visit our Facebook to see more." card.
  - Services on navy: the pool types, then 9 rows. Tapping a row ticks that service in the form; on hover only the arrow fills.
  - Check availability form on paper.
  - Closing band with the big phone number.
  - Footer: name, phone, Facebook.
- **Contact:**
  - The form composes a pre-written text to (848) 480-3729.
  - If messages don't open, a panel offers Copy message and Send it on Messenger. The form also has a call link.
  - The floating text circle appears after the hero and hides while the form is on screen.
- **Checked:** Chromium and WebKit at 360, 390, 430 and 1440 wide.
  - No sideways scroll, tap targets 44px+, the primary button on the first phone screen.
  - The H1 bounce-in shows letters mid-flight early and is restored to the plain heading by 2.5s, on 2 lines.
  - With reduced motion on, nothing is split and nothing is hidden.
  - The circle is hidden on the hero, shown below it and hidden over the form.
  - Form errors and the composed message are correct. No script errors.

## Assumptions I made
- **Services come from the logo badge, not just the brief.** The badge lists opening, closing, cleaning, liner replacement, equipment repairs, acid washes, leak detection and deck coatings, plus "We specialize in building above ground pools". I listed all of them, plus "Above-ground pool builds".
- **Voice is "we"** (an LLC; the caption says "Message us").
- **Colours** are sampled from the logo.
- **The headline** "Your pool, safe all winter." comes from the flyer's "Keep Your Pool Safe This Winter!" and "Peace of mind all winter long".
- **The promise line** uses their own caption ("Message us today to ask about availability"). The earlier "We'll find you a day before the freeze" promised availability they never stated, so it's gone.
- **About copy is mine, in their voice:** "We close your pool like we'll be the ones opening it in spring, because we'd like to be." The facts behind it are theirs: new in 2026, 10+ years' experience, above-ground specialty.
- **Not used:** "Reliable and affordable" (it reads like any company's line) and the flyer image (a promo graphic, not work).

## Placeholders and gaps
- **No real job photos anywhere** (Facebook has only promo graphics). There's no photo/proof section; the logo badge and Facebook link stand in. This is the first thing to add.
- **Why the hero has no photo** (photo-hero rule, 2026-10-19): there are none to use. The only images are the logo badge and an AI-made promo flyer. The flyer's snowy pool scene isn't their work, so putting it behind the hero would pass off a fake as a real job. When the owner sends a real photo (a closing, a liner job, the truck), put it behind the hero under a navy overlay, but only if it looks good in the hero's shape at both 390px and 1440px. Never stretch it, and don't blow a tall photo up into the wide desktop band; if it doesn't fit, keep the colour band. Crop it so the text sits on a quiet area, and sample for 4.5:1 white text.
- **No place in the H1.** The calm style wants the town in the headline, but the brief says the area is unknown and not to infer one. Add it once the owner says where they work (e.g. "Your pool, safe all winter in <town>").
- **No service area** section for the same reason. The form asks for the town.
- **No hours, email, owner name, license/insurance, reviews or prices** on the page.
- **Header logo:** the badge is detailed and unreadable at 44px. The favicon and home-screen icon use a crop of its sun/wave/pool art.
- **Form field fill** is #e6ecf5, as the calm style prescribes. That's visible on the white card but only about 1.2:1, below WCAG's 3:1 for field edges. Labels sit above every field, so I left it.

## Questions for the owner
1. **Does (848) 480-3729 take texts?** The form's main button and the floating circle both send a text. If it's a landline, switch both to copy the message and open Messenger (`https://m.me/61572061220492`).
2. Which towns do you cover? That puts the place in the headline and adds a service-area line.
3. Photos of real closings, openings, liner jobs or above-ground builds, and any before/afters.
4. Your first name, for the About section ("I'm ___, and…").
5. Hours, and whether you're licensed and insured.
6. Any customer reviews we can quote word for word.
7. An email for the footer, if you want one.
8. Which services matter most after closing season? The order could change by season (openings first in spring).

## Ideas not built (yours to pick)
- **Opt-in signature motion (runner-up):** the earlier interactive pool hero. It had clear water with moving light, autumn leaves, and a skimmer net you drag to scoop them, plus moving waterlines between sections. It's at commit `7560319`. The other world considered was frost forming on a winter cover that your finger wipes clear.
- **"Booking takes a minute." (3 steps) was cut** on the finish reviewer's advice. It repeated the form's lede and the eyebrow, and it put a light band against the light form band. Bring it back on the deep textured band if you want a How-it-works section.
- **Impeccable conflicts kept on purpose:** the eyebrow pills, the H1 letter bounce-in, Cal Sans and the band texture are your chosen calm-style features. Impeccable flags eyebrows and the stripe texture as generated-UI patterns; I kept them and recorded the exceptions in `.impeccable/config.json`.
- Proof photo cards (4:5, from the calm kit) and the "See more of our work on Facebook" row once real photos exist; before/after sliders for a green-to-clear pool.
- Seasonal copy: the hero says "Open clear this spring." in spring.
- The desktop left column under "We service all types of pools." is quiet; proof photos could go there.

## Not verified
- Real-device touch on an iPhone and an Android phone inside Facebook's in-app browser.
- That the `sms:` links open Messages with the body filled on iOS and Android.
- That `m.me/61572061220492` opens a Messenger thread inside the Facebook app. It resolves to a thread over the web; I didn't test it in the app.
- That Cal Sans loads inside Facebook's in-app browser. If it doesn't, the headings fall back to Avenir Next / Segoe UI / system.
