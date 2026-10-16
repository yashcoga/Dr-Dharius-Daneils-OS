# Reference Funnel: Couples OS Summit (live, captured 2026-10-16)

This is the funnel run "a couple of weeks back" for Dr. Dharius and Coach Shameka Daniels. It is the agency's existing visual baseline for this client. Screenshots are in `screenshots/` (desktop at 1440px, plus the opt-in on mobile at 390px).

| Page | URL | What it is |
|---|---|---|
| Opt-in | https://coupleossummit.com/optin | Free 3-day summit registration (couple form) |
| VIP upsell | https://coupleossummit.com/vip-upgrade | **$47** one-time upgrade (closest analog to the RI **$47 Prep Kit**) |
| Platinum upsell | https://coupleossummit.com/platinum | $197 upgrade (shown after VIP purchase) |
| Thank-you | https://coupleossummit.com/thank-you | Registration confirmed and last-chance VIP card |
| VIP confirmed | https://coupleossummit.com/vip-access-confirmed | Post-purchase confirmation |
| Platinum confirmed | https://coupleossummit.com/platinum-access-confirmed | Post-purchase confirmation |

## Structure and copy patterns worth reusing

- **Opt-in:** gold top bar → hero (eyebrow with host names, two-tone Playfair headline, framework word-strip, two short paragraphs, Dates/Time/Location row, countdown, CTA, micro-reassurance) → framework section (5 icon columns) → outcomes ("What You Will Leave With", 3 numbered cards, hosts photo) → audience cards ("Built for Your Relationship Stage") → form section with details card and native GHL form → education disclaimer → footer.
- **$47 upsell:** opens with confirmation and a pattern-interrupt ("WAIT! YOU'RE IN! BEFORE YOU GO…"), then states the offer and price **above the fold** with "One-time payment… Instant access" and an immediate decline link. It names the real problem ("The Three Days Go Well. Then Life Picks Back Up."), uses a without/with comparison and 3 numbered pain points, then a gold quote banner ("A strong relationship isn't built in three days. *It's built in what you do after them.*"), feature cards with product mockups, a Free vs. paid comparison table, and a checkout panel with a summary card. **The decline link is repeated after every CTA.**
- **Thank-you:** a calm, centered single column; check icon; arched host photo; details row; **Add to calendar** and **Share** buttons; a last-chance upsell card; confetti.
- **Confirmation pages:** order summary row (Order / Paid / Covers), "What your upgrade includes" checklist, "What happens next" 01/02/03, details row and calendar button.
- Every page has an education disclaimer: "relationship education, not couples counseling or therapy. Private relationship details are never required in any room."

## Defects spotted (avoid repeating them)

- The live page still shows **Oct 28–30, 2026**, but the summit moved to **Jan 20–23, 2027**.
- **$47** on the upsell vs. **$49** on the thank-you card and the VIP confirmation.
- The /thank-you title has a typo: "Rmegistration confirmed".
- The /platinum-access-confirmed title reads "VIP upgrade confirmed".

## Build notes

- Custom HTML sections inside GHL, plus a native GHL form-builder form (`hl_form-builder`) styled to match.
- An earlier, unused concept build of this page (Cormorant Garamond and Manrope, GSAP and three.js) lives in git commit `df86955` under `dist/`. Those files are deleted from the working tree but recoverable with `git checkout df86955 -- dist/`. That commit also contains `dist/assets/logo.png` (the Couples OS logo).
