# Design System: Dharius Daniels Funnels

Last updated: 2026-10-16. The base is measured from the live Couples OS Summit funnel (computed styles via the browser), which the team calls "our existing branding" for Dharius. The RI direction at the bottom is a **proposal**, not yet approved.

## 1. Base tokens (from coupleossummit.com)

### Color

| Token | Value | Use |
|---|---|---|
| `--navy-900` | `#0B1424` | Footer, deepest band |
| `--navy-800` | `#0F1B2D` | Primary dark background, dark button bg, heading ink on light sections |
| `--navy-700` | `#132340` | Hero gradient top (`linear-gradient(#132340, #0F1B2D)`) |
| `--navy-glass` | `rgba(19,35,64,.72)` | Cards and countdown tiles on dark |
| `--gold-500` | `#C9A86A` | **Primary accent**: buttons, italic heading accents, icon rings, top bar |
| `--gold-600` | `#B08D55` | Gold heading text on light backgrounds (better contrast) |
| `--gold-300` | `#E0C58A` | Small gold labels on dark ("Live now") |
| `--gold-ink` | `#8A6D3B` | Gold eyebrow text on cream |
| `--cream-50` | `#F7F5F1` | Light section background |
| `--ivory` | `#F3F1EC` | Headings and text on dark |
| `--white` | `#FFFFFF` | Cards and form panel |
| `--slate-300` | `#C9D2DF` | Muted text on dark |
| `--slate-400` | `#8FA2BD` | Captions and countdown labels on dark |
| `--slate-500` | `#A9B6C9` | Body copy (light weight) on dark |
| `--slate-600` | `#607179` | Body copy on light |
| `--ink-700` | `#344054` | Form labels |
| `--line` | `#D0D5DD` | Input borders |

### Typography

- **Display:** Playfair Display 500/600, with **italic 500 in gold** for the second line of a headline (e.g. "Love Brought You Together. / *Now Build What Will Carry You Forward.*").
  - H1 hero: 48px / 1.1, letter-spacing −0.015em.
  - H2 section on light: 60px / 1.08, weight 600, two lines with the second line in gold. On dark: 40–46px, weight 500.
  - H3 card titles: 28px, weight 600.
- **Body / UI:** Jost. Body 15px / 24px at weight 300–400; lead paragraphs 17px / 1.55 at weight 300.
- **Eyebrows:** Jost 11–12px, weight 600, uppercase, letter-spacing ~0.2em, gold, often flanked by thin gold rules (`—— THE COUPLES OS FRAMEWORK ——`).
- **Buttons:** Jost 12px, weight 600, uppercase, letter-spacing 0.22em, padding ~16×28, **2px radius** (nearly square). Gold bg with navy text on dark; navy bg with ivory text on light.
- **Form inputs:** Inter 15px, white bg, 0.8px `#D0D5DD` border, square corners, padding 10×20.
- Google Fonts: `Jost:wght@300;400;500;600` and `Playfair+Display:ital,wght@0,500;0,600;0,700;1,400;1,500;1,600`.

### Layout and rhythm

- Content max-width **1100–1160px**; text columns 520–620px; centered intros ~900px.
- Section padding: hero 96/104px; light sections 72–80px; dark sections 88px. Side padding 32px desktop.
- **Alternating bands:** dark navy hero → cream section → navy section → cream section → navy form section → deep-navy footer.
- Thin gold top announcement bar (11px uppercase, letter-spaced).
- Rich imagery: **background-removed cutouts** of the hosts on navy, an arched frame with a thin gold outline (thank-you page), and soft vignettes and glows.
- Repeated **countdown** blocks (Days / Hrs / Min / Sec tiles) with a CTA after each major section.
- A **sticky slim header** appears near the form (logo, date line, mini countdown, CTA).
- Numbered items use gold circles with italic Playfair numerals (01 / 02 / 03).
- Icons: navy circles with a gold outline ring and line icons.
- Subtle motion: confetti on the thank-you page; gentle reveals.

### Page patterns already proven in this funnel

- **Opt-in:** hero (copy left, host cutout right) → framework strip (5 icons) → outcomes (photo left, numbered list right) → audience cards → form section (copy and photo left, white form card right).
- **$47 upsell:** gold top bar "WAIT! YOU'RE IN!…" → headline and CTA → product mockup → "Let's be honest…" problem → without/with comparison → 3 numbered pains → gold banner quote → "One Upgrade. Four Ways…" 2×2 feature cards with mockups → Free vs VIP table → checkout panel (summary card left, order form right) → decline link repeated.
- **Thank-you:** gold bar → check icon → headline → arched host photo → details row → Add to calendar and Share buttons → last-chance upsell card.

## 2. Photography

PD solo shots for RI (warm tan studio backdrop; all need **background removal** to sit on navy the way the Couples OS cutouts do):
- Navy denim jacket set: `daniels-7747` (seated, hands clasped; authoritative), `daniels-7755` (seated, relaxed), `daniels-7800` (standing, warm smile), `daniels-7792` (standing, laughing, hands together).
- Tan jacket set: `daniels-7996` (standing, confident), `daniels-7998` (looking up, joyful).

Index: [assets/headshots/README.md](../assets/headshots/README.md).

## 3. Proposed RI direction (for discussion)

RI is a **separate offer** for **individuals**, so it should feel like Dr. Daniels's world, not a Couples OS spin-off, while keeping the same foundation so it reads as one brand family.

- **Keep:** Playfair Display with Jost, the gold accent, the 2px buttons, the eyebrow style, the countdown, the alternating rhythm, and the italic gold second line.
- **Shift the mood:** lead with the **cream/ivory** ground and use navy as the contrast band (more personal and reflective). The tan studio backdrop in PD's photos pairs naturally with warm cream, so cutouts may not be needed on light sections.
- **Signature visual ideas** tied to the message (pick 1–2, don't overdo it):
  1. **Deposits vs. withdrawals:** a ledger or balance motif ("You: ████████ / Them: ██") for the upside-down problem.
  2. **"Upside down":** a headline word or icon literally inverted for Version C, then turned "right side up" in the solution section.
  3. **The five seats:** a seat or table diagram (five chairs around a table), each labeled, with Family marked as new and no criteria shown.
  4. **Evaluate → Place → Manage:** a 3-step progression with gold numerals.
- **The book as a hero object:** a 3D book mockup next to PD (needs the cover file).
- **Per-variation accent:** the same layout system, with a different hero headline treatment and a different hero photo for A/B/C, so the test measures the message rather than the layout.
