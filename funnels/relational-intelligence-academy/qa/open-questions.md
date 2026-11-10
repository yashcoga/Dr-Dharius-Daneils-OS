# Academy sales page: open questions

Questions to send to the client team. When the list is complete, turn it into a PDF with a screenshot of each spot on the page next to its question.

Page preview: https://sites.leadconnectorhq.com/preview/IO0cRnJpTem584LlDDxC
Code: `ghl/AcademySalesPage-ghl.html`

## Parked

4. **Coaching call schedule** (welcome page, step 2)
   - Text: "Live coaching calls are on November 17, November 24, December 3, December 10, December 15 and December 17."
   - Question: Are these the right dates, and what time is each call? They switch between Tuesday and Thursday, and there are 2 calls in the week of Dec 14 but none in the week of Dec 1. The sales page mock-up says "Thursday · 8 PM ET".
   - Status: parked (from the Nov 2 funnel audit).

5. **Welcome page details** (welcome page)
   - Text: "[PLATFORM]", subject "[INSERT]", "[Add to calendar links]", "second payment will be charged on [DATE]", welcome video.
   - Question: Which platform hosts the Academy, what is the login email's subject line, when is the second 2-pay payment charged, and is the welcome video ready?
   - Status: parked.

6. **2-payment option** (sales page)
   - Question: Should /academy link to the 2-payment page (/academy-2-pay)? Right now the page promises "2 payment option" but nothing links to it. And is the Whop 2-pay plan set to stop after 2 payments?
   - Status: parked.

7. **AI Agent** (sales page, Bonus 1)
   - Question: Is the Relational Intelligence AI Agent confirmed and ready for November 17?
   - Status: parked.

8. **"Ministry" in the FAQ** ("Is this only for romantic relationships?")
   - Question: Is Dr. Daniels happy with "ministry" in the list of relationships?
   - Status: parked.

## Added Nov 3 (live /academy page review)

Full feedback: `academy-optin-feedback.html` and the matching PDF. Items 6–8 above are still open on the live page (2-pay not linked, "ministry" still in the FAQ).

9. **Live call time zone** (laptop mockup vs share image)
   - The page mockup says "Thursday · 8 PM **ET**"; the share image says "Thursday · 8 PM **CT**". Nov 17 is a Tuesday, so if calls are Thursdays the first call is Nov 19. Which is right? (Ties to item 4.)
10. **Repositioning Clinic date** (Bonus 9): when is the group session?
11. **Company name in the footer**: the footer says "© 2026 Dr. Dharius Daniels"; the legal pages and SMS consent say "Relationship Operating System, LLC". Which entity?
12. **Tracking**: no Meta pixel or Google tag loads on /academy. Is tracking planned?
13. **Tone (for Dr. Daniels)**: keep "Managing Separation and Elimination" (Week 6) and "the three relationships costing you the most" (Week 1)?
14. **Testimonials**: any approved quotes from masterclass attendees, readers or coaching members?

## For the developer (config.php on aibotxpert.com), added Nov 10

Do this before the new checkout code goes live.

| Offer | Plan ID | Page |
|---|---|---|
| `full` | `plan_7YN2PaFTNCgQs` | /academy-checkout ($597) |
| `twopay` | `plan_nbXH8fSLIXs6K` | /academy-checkout-2-pay (2 x $327) |
| Certification upsell (`upsell.php`) | `plan_o8dmQjp7oYiuK` | /certification-upgrade-1 ($1,000, one-time) |

- Replace the test plans if they are still set (`plan_Stepb8xJSmTdv`, `plan_ruVNCWeF1ZHIB`).
- Confirm the server is using the live Whop account, not test mode.

## Resolved (not for the PDF)

- **[OPTIONS]** (Michael, Nov 3): "ClarityPay and Sezzle". Klarna and AfterPay may be added later; Michael will confirm.
- **[REASON FOR THE DEADLINE]** (Michael, Nov 3): "We have orientation for new members that week."
- **[TIME PER WEEK]** (Michael, Nov 3): "1 to 2 hours per week."
- These three are live on /academy and in `design/academy-sales.html`.

- **[SUPPORT EMAIL]**: use info@workwiththedaniels.com (same as the legal pages). The funnel designer is adding it.
