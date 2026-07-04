# L.I.N.K. Portfolio — Design Specification

**Version:** 0.1 (for review)
**Source:** Extracted from the three L.I.N.K. tool mockups — `cstar-mockup-v2.html`, `how-to-hub-mockup.html`, `LINK_Task_Builder_v2.html`.
**Purpose:** Lock the visual design language the portfolio site inherits, *before any site code is written*. This is my read of the shared language across the three tools, with every disagreement between them flagged for your decision rather than silently resolved.

**Status:** ✅ APPROVED + LOCKED (Drizzy, 04 JUL 2026). All conflicts C1–C8 resolved — see §7. The token set in §8 is final and the site builds against it.

---

## 0. The one-line read

All three tools are the same product family: a **dark "charcoal console" UI with a single gold accent.** Near-black background, charcoal cards, one saturated gold (`#FFCD00`) carrying every emphasis — headings, active states, primary buttons, focus rings, brand. Segoe UI type. Geometric, dense, military-utility feel. Gold-on-charcoal is the entire identity; color is used sparingly and with intent.

The portfolio inherits this verbatim. Where a portfolio (a marketing-ish landing page) needs something the tools didn't have — a hero, generous vertical rhythm, section spacing for a scrolling page rather than a fixed app shell — I'll extend the language, but the palette, type, and component styling below are the anchor.

---

## 1. Color palette

Legend: ✅ = all three agree · ⚠️ = they disagree (your call in §7).

| Role | Token seen | C-STAR | How2Hub | Task Builder | Agree? |
|---|---|---|---|---|---|
| **Accent / gold** | `--gold` | `#FFCD00` | `#FFCD00` | `#FFCD00` | ✅ |
| **Line / border** | `--line` | `#474747` | `#474747` | `#474747` | ✅ |
| **Muted text** | `--muted`/`--mute` | `#9a9a9a` | `#9a9a9a` | `#9a9a9a` | ✅ |
| **Card surface** | `--charcoal`/`--card` | `#333333` | `#333333` | `#333333` | ✅ |
| **Page background** | `body` | `#1e1e1e` | `#1e1e1e` | `#262626` | ⚠️ TB lighter |
| **Body / primary text** | `--offwhite`/`--ghost` | `#F2F2F2` | `#F2F2F2` | `#F8F8FF` | ⚠️ TB is blue-white |
| **Header bar** | header bg | `#333333` | `#333333` | `#2e2e2e` | ⚠️ TB darker |
| **Raised surface** | `--charcoal-2` | `#2a2a2a` | `#2a2a2a` | `#2b2b2b`/`#2f2f2f` | ⚠️ minor |
| **Hover surface** | `--charcoal-3` | `#3d3d3d` | `#3d3d3d` | (uses transparent+border) | ~ |
| **Success / green** | `--green` | `#6fbf73` | — | `#63d68b` | ⚠️ two greens |
| **Danger / red** | `--red`/`--danger` | `#e06c6c` | — | `#ff5b5b` | ⚠️ two reds |
| **Warning / amber** | `--amber` | — | — | `#ffb84d` | TB only |

**Task Builder frequency palette (semantic status colors, TB only):**
Daily `#ff5b5b` (red) · Weekly `#FFCD00` (gold) · Monthly `#63d68b` (green) · Quarterly `#4aa3ff` (blue) · Non-Recurring `#cfcfcf` (grey). These are a data-encoding legend, not general UI color — likely irrelevant to the portfolio, but noted so nothing is lost.

**My read:** the "canonical" palette is the C-STAR / How2Hub set (two of three agree on nearly everything). Task Builder drifts a few hex values lighter/bluer. I recommend standardizing on the C-STAR/How2Hub values — but the green and red genuinely differ and the portfolio only needs them if we show status color at all (e.g. measured-vs-baseline, projection labels). See §7.

---

## 2. Typography

| Attribute | Value | Notes |
|---|---|---|
| **Primary family** | `'Segoe UI', -apple-system, Tahoma, Arial, sans-serif` | ✅ all three (Task Builder drops `-apple-system`, adds `Arial`; C-STAR/How2Hub include `-apple-system`). Merge = the line at left. |
| **Monospace** | `Consolas, monospace` | Task Builder only — IDs, JSON peek, numeric fields. Available if the portfolio wants a "system/technical" mono accent (e.g. flow counts, taskIds). |
| **Brand wordmark** | gold, `700`, `letter-spacing: 2–2.5px`, ~15–20px, often uppercased | ✅ consistent treatment |
| **Section label** | gold, `700`, `letter-spacing: 2px`, `text-transform: uppercase`, ~12–13px | ✅ the signature heading style. See §5 for the divider variants. |
| **Panel/page title** | gold, `700`, 25–27px (C-STAR 25, How2Hub 27, TB hero 26/ls 3px) | ✅ big gold title is the pattern |
| **Body copy** | offwhite, 14–15.5px, `line-height` ~1.5–1.6 | ✅ |
| **Muted sub/hint** | muted grey, 11–13px, often `letter-spacing: 0.5–1px` | ✅ |
| **Numeric emphasis** | bold, often gold | ✅ (funnel counts, contracts, stats) |

No web fonts are loaded anywhere — everything is a system font stack. **Recommendation:** keep it system-font (fast, no external request, on-brand for a government-adjacent utility). If you want a touch more "designed" feel for the hero headline only, flag it in §7 and I'll propose one self-hosted display face — otherwise Segoe stack throughout.

---

## 3. Spacing, radius, borders

| Attribute | C-STAR | How2Hub | Task Builder | Resolved (proposed) |
|---|---|---|---|---|
| **Header height** | 64px fixed | 64px fixed | ~50px (12px padding) | ⚠️ §7 — 64px reads as the standard |
| **Card radius** | 8px | 8px | 12px | ⚠️ §7 — 8 vs 12 |
| **Button radius** | 7px | — | 8px | ~8px |
| **Input radius** | 5–6px | 6px | 8px | ~6–8px |
| **Chip / pill radius** | 18px | 18px | 999px | fully round (same intent) ✅ |
| **Icon-box radius** | 6–7px | 6px | 7px | 6px ✅ |
| **Card padding** | 14–20px | — | 20–22px | ~20px |
| **Content max-width** | 820–1000px | — | 920px | 900–1000px |
| **Border weight** | 1px `--line`; 2px gold underlines/accents | same | same | ✅ 1px hairlines, 2px gold accents |
| **Left-accent bar** | 3px gold on active/selected | 3px gold | — | ✅ 3px gold active indicator |

**Consistent spacing instincts across all three:** hairline `#474747` borders everywhere, generous internal padding, gold used as a *2px* structural accent (header bottom-border, active left-border, focus ring) vs *1px* neutral lines for everything else.

---

## 4. Component styling (shared vocabulary)

These are the reusable pieces the portfolio should be built from:

- **Header bar** — full-width, charcoal, **2px gold bottom border**, brand at left, a context "chip" at right (`role-chip` in the tools — "Viewing as Station Commander"). Portfolio analog: nav with the L.I.N.K. mark at left, section anchors / Contact CTA at right.
- **Brand mark** — a **38×38 rounded square, 2px gold border, gold monogram "LNK" centered, weight 800.** Present in C-STAR + How2Hub headers. (Task Builder uses a text-only wordmark, no box.) *This is the leading candidate for the site icon — see §6.*
- **Section label** — gold uppercase tracked label. Two divider treatments differ (§5).
- **Cards** — charcoal `#333`/`#2a2a2a`, 1px line border, rounded, often a **3px colored left-border** to signal type (e.g. C-STAR RCA card = red left border for "problem"). Portfolio: component cards, competency rows, roadmap lines.
- **Chips / pills** — rounded, 1px line border; **"armed/active" = solid gold fill + charcoal text + weight 700.** Used for tags, filters, selectable options. This gold-fill-on-active is the single most repeated interaction signal.
- **Buttons** — `.primary` = solid gold, charcoal text, weight 700. `.secondary/.ghost` = transparent, line border, hover → gold border + gold text. ✅ identical logic all three.
- **Inputs / selects / textareas** — dark fill, 1px line border, **focus → gold border** (no glow). ✅
- **Steppers / progress** — numbered dots; **active = gold fill/charcoal text**, done = gold outline + check, todo = grey outline. C-STAR (vertical rail) and Task Builder (horizontal top) both use it. Useful pattern for the site's guided-tour / story progression.
- **Note / callout box** — `background: rgba(255,205,0,0.06)`, **3px gold left border**, muted text. ✅ The "placeholder / caveat" voice. Perfect for the *"Projected — labeled as projection"* copy rule and the screenshot placeholders.
- **Table / funnel rows** — grid rows, uppercase muted header row on `#2a2a2a`, hairline row dividers, right-aligned status flags (green "On Track" / red "Below"). Good basis for the Numbers Ledger and rollout timeline.
- **Two-pane detail layout** — left rail (nav/gallery/steps) + right detail panel. Both C-STAR and How2Hub use it. **This is the exact pattern for Section 7's system map** (map/nodes ↔ side detail panel).
- **Status flag pill** — small rounded pill, colored text on 12%-opacity colored bg (`.ok` green, `.low` red). For measured-vs-baseline framing.
- **Scrollbar** — thin (8–9px), thumb = `--line`, track invisible. Minor but consistent.

---

## 5. Iconography & the divider question

**Icon system is 100% CSS + Unicode/emoji glyphs — there are zero image/SVG asset files in any mockup.** That matters for the site icon (see §6): whatever you pick, I reproduce it in CSS/SVG, not by extracting a file.

**Divider treatment — a real conflict:** the gold section label has two different underline styles:
- C-STAR / How2Hub: label text, then a **flex-fill 1px line to the right** (`::after` rule that extends across remaining width).
- Task Builder: label text with a **full-width `border-bottom` under it.**

Both are "gold-tracked label + hairline rule," just different geometry. §7 asks which.

---

## 6. Icon / logo asset inventory — **pick the site icon**

Per your instruction, here is *every* icon/logo/glyph asset found across the three mockups. You identify which one is the site's required icon (favicon + hero mark); it gets used as-is.

**Brand / logo marks:**
1. **"LNK" monogram box** — 38×38 rounded square, 2px gold border, gold "LNK" letters (weight 800), centered. Appears in **C-STAR and How2Hub** headers. *(My default guess for the site icon.)*
2. **"L.I.N.K." gold wordmark** — the spelled-out gold tracked lettermark (Task Builder brand text; also the `brand-title` treatment). A wordmark, not a compact icon.

**Functional glyphs (Unicode geometric — used as task/category/action icons):**
3. **▲** up-triangle — C-STAR recommendation icon *and* How2Hub "NCOER". Reads as "action / recommendation."
4. **★** star — How2Hub "Future Soldier Training Program."
5. **◆** diamond — How2Hub "Production Counseling."
6. **▦** grid/square — How2Hub "Planning Meeting."
7. **●** filled circle — How2Hub "GOV Logs."
8. **▸ / ▶** right-triangle bullet (U+25B8) — Task Builder resource bullets; chevrons `›` in How2Hub lists.
9. **🔻** red down-triangle (U+1F53B) — Task Builder plain-text export title marker.
10. **🔹** small blue diamond (U+1F539) — Task Builder section marker.

**Emoji utility icons:**
11. **📁** folder — resources (How2Hub button, Task Builder).
12. **🔍** magnifier — search field.
13. **⌂** house (U+2302) — Task Builder "Start / home" button.
14. **👤** bust — Task Builder role marker.

**Status-dot system (colored circles):**
15. Frequency dots 🔴🟡🟢🔵⚪ / colored `<span>` dots — Task Builder + C-STAR calendar legend. A system, not a single mark.

> **RESOLVED (Drizzy, 04 JUL 2026):** the site icon is none of the mockup glyphs — it is the **gold compass rose mark** supplied separately: `Compass logo LINK.png` (1024×1024 PNG, gold rose with N/W/E cardinals, "L.I.N.K." wordmark beneath, on near-black ~#111 background). **Used as-is for favicon and hero mark. LOCKED, non-negotiable.**
>
> Practical notes (file untouched, these are page-side accommodations only):
> - The PNG background is solid near-black (~`#111`), not transparent. The hero places the mark on a matching near-black field so no square edge shows; at favicon size the dark square reads as intended on any tab bar.
> - The compass rose is a perfect thematic fit: L.I.N.K. = Leader's Integration and **Navigation** Kit.
> - The mockup "LNK" monogram box (§6 item 1) remains available as the compact in-page nav mark if the full compass PNG is too heavy for the sticky header — flagged as an open styling call for the hero A/B round, not resolved here.

---

## 7. Conflicts — ALL RESOLVED (Drizzy, 04 JUL 2026)

**C1 — Page background.** ✅ `#1e1e1e` (C-STAR/How2Hub majority).

**C2 — Primary text white.** ✅ `#F2F2F2`.

**C3 — Header background.** ✅ `#333333` with the 2px gold underline.

**C4 — Card corner radius.** ✅ **12px.**

**C5 — Status color.** ✅ **Green/red allowed, softer C-STAR pair** (`#6fbf73` / `#e06c6c`). Explicit intent: *the 90%-vs-13% turnaround must read visually.*

**C6 — Section-label divider.** ✅ Flex-fill line to the right.

**C7 — Hero headline font.** ✅ System Segoe stack only, no web fonts.

**C8 — Site icon.** ✅ `Compass logo LINK.png` (gold compass rose), used as-is, favicon + hero mark. See §6.

---

## 8. LOCKED token set (final — the site builds against this)

```css
:root{
  /* surfaces */
  --bg:        #1e1e1e;   /* page */
  --surface:   #2a2a2a;   /* raised panels / rails */
  --card:      #333333;   /* cards, header */
  --hover:     #3d3d3d;   /* hover fill */
  /* ink */
  --gold:      #FFCD00;   /* the accent — headings, active, primary, focus */
  --text:      #F2F2F2;   /* primary */
  --muted:     #9a9a9a;   /* secondary / hints */
  --line:      #474747;   /* hairline borders */
  /* status (only if used; softer pair) */
  --green:     #6fbf73;
  --red:       #e06c6c;
  /* type */
  --font:  'Segoe UI', -apple-system, Tahoma, Arial, sans-serif;
  --mono:  Consolas, ui-monospace, monospace;
  /* geometry */
  --radius-card: 12px;
  --radius-ctl:  8px;
  --radius-pill: 999px;
  --accent-bar:  3px;   /* gold active left-border */
  --gold-underline: 2px;
}
```

**Design principles carried from the tools (guardrails for the build):**
1. **One accent.** Gold is the only saturated color. If everything is gold, nothing is — spend it on headings, active state, primary action, focus.
2. **Hairlines, not boxes.** 1px `#474747` borders define structure; avoid heavy fills.
3. **Gold-fill = "this is on."** The single consistent interaction signal (active chip, current step, primary button).
4. **The note box is the honesty voice.** Gold-tinted left-border callout = every "projected / placeholder / caveat" moment (directly serves the blueprint's projection copy rule and the 7 screenshot placeholders).
5. **Two-pane = the map.** Left selector ↔ right detail panel is already the house pattern; the Section 7 system map is built on it.

---

### Step 2 status
Spec approved in full. Next gate: two hero directions (`hero-direction-a.html`, `hero-direction-b.html`) — same locked palette, differing layout and tone. Drizzy reviews both in-browser locally and locks one direction before any further site code.
