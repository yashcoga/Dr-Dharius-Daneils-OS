# Funnel: SinglesOS (trademark landing page)

Status: **first design ready for review** (2026-11-03). Requested for the SinglesOS trademark filing for Dr. Dharius Daniels. The attorney needs a simple live page that shows the name with the services.

Two versions of the same one-page site, for the client to choose between:

| Version | Look | Copy | Design |
|---|---|---|---|
| A | Navy hero, copy left and photos right, arch-mark logo. Headline: "Single Isn't a Waiting Room." | `copy/landing.md` | `design/singles-os.html` |
| B | Longer page: centered copy on a dark hero with a photo on each side (hero option 3, chosen 2026-11-03; the other options are in `design/_options/`), "Meet your hosts", "Sound familiar?" and "Ways to learn" sections, gold "OS" badge logo. Headline: "Know Who You Are Before You Choose Your Partner." | `copy/landing-b.md` | `design/singles-os-b.html` |

Both use the same services line, photos, bios and footer, and neither has a form. Screenshots: `qa/shots/a-*` and `qa/shots/b-*` (desktop at 1440px; phones at 390px and 360px). Checked: no sideways scroll on phones, and buttons are full width and 56px tall.

To view: open either HTML file in a browser (keep `design/assets/` next to it).

## Next steps
1. Review the page, then send it on for the attorney.
2. Domain: to be confirmed.
3. Build it in GHL (`html-to-ghl` skill) and upload the two photos from `design/assets/`.
4. Once it's live, share the live URL and the date it went live (trademark filings usually need a live page, not a mock-up).

```
copy/     page copy
design/   standalone HTML page + photos
ghl/      GHL code block (after approval)
qa/       screenshots and checks
```
