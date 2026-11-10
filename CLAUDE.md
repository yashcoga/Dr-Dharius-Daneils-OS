# Working in this folder

This is the client operating system for **Dr. Dharius Daniels** ("PD" internally; never use "PD" in customer-facing copy). We build his funnels (copy and design) for GoHighLevel. See [README.md](README.md) for the map.

## Before writing copy or designing anything

1. Read `brain/02-offer-and-event.md` and `brain/03-voice-and-messaging.md`. They hold the facts and the compliance rules.
2. For design, read `design/design-system.md` and look at `reference/couples-os-summit-funnel/screenshots/`.
3. Check `brain/06-open-items.md` for what is still unconfirmed.

## Non-negotiables

- **Banned photo: never use headshot `daniels-7747`** (seated, hands clasped between the knees, straight face) or any crop or cutout of it (`pd-7747*`), in any funnel, page, email or ad. Dr. Daniels doesn't like it (client feedback, 2026-11-03). In every design, review or audit, check every photo of him (also images hosted on GHL, which have different file names) and **flag any use of it as the #1 fix**.
- **The coach's photo always faces the copy.** If he looks or turns left, put the photo to the right of the text, and the other way round.
- **Education, not therapy or counseling.** Never promise to fix relationships or guarantee how others respond.
- **Never invent** the Family seat's criteria, the Prep Kit teaching title, or any 6-week program detail (name, price, inclusions, schedule, refund). Use `[PLACEHOLDER]`s.
- **No promises** of private PD access, individual answers, AI tools, unconfirmed bonuses, or a results guarantee. Certification only as the client defined it on 2026-11-10 (Academy + RI Certification, $1,597; see `brain/02-offer-and-event.md`): never a license, never an earnings promise.
- The **Relational Intelligence** offer is for **individuals** and is **separate from Couples OS**. Don't carry over couple language, and keep Shameka off RI pages.
- Event: **Tuesday, November 10, 2026, 7:00 PM ET**, free, live online. The Prep Kit is **$47**, one-time, with a 30-day refund (kit only). Keep the date, time and price identical on every page (the reference funnel has $47/$49 mismatches; don't repeat that).
- The book title is always italic: *Relational Intelligence: The People Skills You Need for the Life of Purpose You Want*.

## Conventions

- **The GitHub repo is public** (github.com/yashcoga/Dr-Dharius-Daneils-OS, view-only for others). Internal or sensitive material (team contacts, internal links, strategy, onboarding data) goes in the local-only files listed in `.gitignore`, never in tracked files. Scan before every push.

- New funnel work lives in `funnels/<funnel-name>/` (copy/, design/, ghl/, qa/).
- Source docs in `reference/source-docs/` are dated snapshots. Drive is the source of truth, so re-pull before finalizing.
- When facts change, update the relevant `brain/` file and its "Last updated" date rather than adding new scattered notes.
- Use the `html-to-ghl` skill to port finished HTML into GHL and the `funnel-audit` skill for pre-launch QA.
- **Every page update gets a timestamp, inside the page itself.** Each GHL code file starts with an `UPDATE LOG` HTML comment (not shown on the page). On every change, add an entry at the top of its list: `YYYY-MM-DD HH:MM IST | Name`, then short `- ` pointers for what changed (name is "Yash" for work done with Yash). No separate changelog file. Keep it free of internal or sensitive details, since it's visible in the live page source. (Started on the Replay page, 2026-11-10.)
