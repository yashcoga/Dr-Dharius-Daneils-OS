# Funnel Map: RI Masterclass (front end)

Last updated: 2026-10-16. Platform: **GoHighLevel**. Domain and URLs: ⛔ not decided.

## Page flow

```
[Ads / organic / warm list]
        │
        ├── Reg A: Give Without Going Empty ─┐
        ├── Reg B: Break the Pattern ─────────┼──► $47 Prep Kit offer ──► Checkout ──► Thank-you page
        └── Reg C: Upside-Down Relationships ─┘            │                              ▲
                                                           └──── "No thanks" ─────────────┘
```

| # | Page | Purpose | Copy status | Notes |
|---|---|---|---|---|
| 1a/b/c | Registration A/B/C | Free seat opt-in | 🟡 full copy drafted | Same form and same next page. **Each variation must write its own event name into `contact.ri_masterclass_name`** (the emails use it). |
| 2 | Prep Kit offer ($47) | One-time offer after opt-in | 🟡 full copy drafted | Confirmation bar at top: "You're registered… Don't close this page yet." Decline link → thank-you page. |
| 2b | Prep Kit checkout | Payment | ⛔ no processor yet | Could be a GHL one-click order form on page 2 (like the Couples OS VIP page) or a separate checkout step. The brief describes it as a separate checkout. |
| 3 | Thank-you page | Confirm, calendar, prep, share | 🟡 full copy drafted | Shared by buyers and non-buyers. Copy mentions both emails. |
| later | Main-offer sales page and checkout | 6-week program | ⛔ awaiting offer sheet | Out of scope until the offer is locked. |

## Form spec (all three registration pages)

| Field | Required | Notes |
|---|---|---|
| First name | ✅ | |
| Email | ✅ | |
| Mobile number | optional | "For text reminders." |
| SMS consent checkbox | optional, unticked | "Yes, send me masterclass confirmation and reminder texts from [SENDER NAME]. Message frequency varies. Message and data rates may apply. Reply STOP to opt out or HELP for help. Consent is not required to register. [TERMS] [PRIVACY POLICY]" |
| Hidden: variation | auto | Set `ri_masterclass_name` and a variation tag (A/B/C) for the test. |

Button: **SAVE MY FREE SEAT**. Under it: "We'll email your confirmation, access details, and reminders. No payment or book purchase required."

## GHL custom values and fields used by the email/SMS copy

| Merge field | Type | Value |
|---|---|---|
| `{{contact.first_name}}` | contact | |
| `{{contact.ri_masterclass_name}}` | **contact** field | "Give Without Going Empty" / "Break the Pattern" / "Upside-Down Relationships", depending on the page they registered on |
| `{{contact.ri_masterclass_join_url}}` | **contact** field | Personal join link (per registrant, for example a Zoom webinar registrant link) |
| `{{custom_values.ri_masterclass_date}}` | custom value | Tuesday, November 10 |
| `{{custom_values.ri_masterclass_time}}` | custom value | 7:00 PM |
| `{{custom_values.ri_masterclass_timezone}}` | custom value | ET |
| `{{custom_values.ri_support_email}}` | custom value | ⛔ TBD |
| `{{custom_values.ri_sms_sender_name}}` | custom value | ⛔ TBD |
| `{{custom_values.ri_teaching_title}}` | custom value | ⛔ TBD (PD to choose) |

Agency template note: all emails end with `{{custom_values.email_footer}}`.

## Registrant email/SMS schedule (from the email doc; times in ET, event Tue Nov 10, 7 PM)

| When | Email | SMS |
|---|---|---|
| Immediately | Confirmation: "You're registered. Your masterclass details are inside." | "You're registered…" (consent only) |
| +~2 hrs | Reply-focused: "What are your relationships costing you?" | |
| −12 days, 10 AM (Oct 29) | "They need you. But do you feel supported?" | |
| −10 days, 10 AM (Oct 31) | "You've known them for years. What has that shown you?" | |
| −7 days, 10 AM (Nov 3) | "You can hope they change. But what do you do today?" | |
| −5 days, 10 AM (Nov 5) | "You are important to me. But you're not the only important thing." | |
| *Alt:* +24 hrs for late registrants | Condensed nurture: "Before we meet, look at what you've been carrying" (**instead of** the 4 above) | |
| −3 days, 10 AM / 12 PM (Nov 7) | "Bring three relationships to mind" | 3-day SMS at 12 PM |
| −1 day, 7 PM (Nov 9) | "Tomorrow: your masterclass access" | Tomorrow SMS |
| Day-of 4 PM | "We start in three hours. Here's your link." | |
| Day-of 6 PM | "We begin in one hour" | 1-hour SMS |
| Day-of 6:45 PM | 15-minute email **or** SMS (not both) | |
| Day-of 7 PM | "We're live. Join me now." | Live SMS |
| Day-of 7:10 PM (optional) | Not-yet-joined email **or** SMS | |
| On Prep Kit payment | "Your Relational Intelligence Prep Kit is ready." | |

Separate assets exist but **were not shared with us**: the warm-list promo (6 emails and 4 SMS), the 45 ad scripts and the GHL tag reference.

## Suggested tags (following the agency's template naming; the final list belongs to the CRM team)

`RI - Masterclass Nov10 - Registered` · `RI - Masterclass Nov10 - Reg A` / `Reg B` / `Reg C` · `RI - Masterclass Nov10 - SMS Opt-In` · `RI - Prep Kit - Purchased` · `RI - Prep Kit - Refunded` · `RI - Masterclass Nov10 - Attended` · `RI - Masterclass Nov10 - Watched Replay` · `RI - Program - Purchased`

## Build pattern (copied from how the live Couples OS funnel is built)

- Page sections are **custom HTML/CSS code blocks** inside GHL (classes like `.hero`, `.section-light`, `.outcomes`).
- The **registration form is GHL's native form builder**, styled to match, so contacts, tags and workflows work natively.
- The countdown is a custom JS block targeting the event date and time (Nov 10, 2026, 7:00 PM ET, which is `2026-11-10T19:00:00-05:00`).
- Use the `html-to-ghl` skill when converting a designed HTML page into a GHL code block.
- Use the `funnel-audit` skill for pre-launch QA (desktop and mobile, pixels, legal links, test purchase).
