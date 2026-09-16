---
name: "TDNA — Taiwan Digital Nomad Association"
category: Brands
surface: web
colors:
  background: "#F6F6F6"
  surface: "#FFFFFF"
  foreground: "#1E1F1C"
  muted: "#66685F"
  border: "#DCDDD8"
  accent: "#004E9D"
  accent-secondary: "#FFD028"
  accent-tertiary: "#10B8D9"
  pink: "#F9D2E5"
  orange: "#E74310"
  green: "#00993E"
  red: "#E4003D"
  plum: "#C54090"
---

# TDNA — Taiwan Digital Nomad Association Design System

> Category: Brands
> Surface: web, admin UI, social, deck, print
> Owner: 台灣數位遊牧者協會 Taiwan Digital Nomad Association (TDNA) · 《品牌視覺系統 VI 2.1》Aug 2024, designed and compiled by 呂罰 Kipha Lu
> A structured, stable, quietly playful system: slab-serif `TDNA` mark, ten fixed CIS colours, Figtree + Noto Sans TC on screen, white panels on light-grey paper, square corners, a hard 4px offset shadow and one 10px yellow spine. The same semantic tokens run admin.dna.org.tw, hub.dna.org.tw and cis.dna.org.tw.

## Brand and voice

- TDNA integrates government and industry resources so digital nomads succeed in career growth and exchange: skills training, startup resource links, career guidance, community events and forums. Keywords: **數位 · 創意 · 實驗** (digital, creative, experimental).
- Name forms: `TDNA` (mark and short form), `台灣數位遊牧者協會` (Chinese full name), `TAIWAN DIGITAL NOMAD ASSOCIATION` (English wordmark, always uppercase in lockups). In running text: Taiwan Digital Nomad Association.
- Voice: plain, direct, organised, warm. Taiwan Traditional Chinese wording (軟體、程式、資料、網路、活動、報名); never Simplified characters or mainland terms. English is sentence case except the wordmark. State dates, places, cost and limits plainly; CTAs are verbs (加入會員、報名、看活動、儲存).
- TDNA also hosts Taiwan Digital Fest (TDF); that event has its own system (`tdf-2027`). Do not mix TDF's black Mondrian rules and pixel type into TDNA material; when TDNA endorses an event, place the TDNA lockup as a quiet endorsement line.

## Colour

Ten official CIS colours. Print uses CMYK, screen uses HEX. Values never change; do not add tints by hand or gradients.

| Role | Name | HEX | CMYK | Token | Text on it |
| --- | --- | --- | --- | --- | --- |
| Primary fill | 黃 Yellow | `#FFD028` | 0,19,88,0 | `--tdna-yellow` / `--tdna-spine` | ink |
| Primary fill | 青 Cyan | `#10B8D9` | 71,0,13,0 | `--tdna-cyan` | ink |
| Primary fill | 粉 Pink | `#F9D2E5` | 0,25,0,0 | `--tdna-pink` | ink |
| Fill | 橘 Orange | `#E74310` | 0,84,100,0 | `--tdna-orange` | white, display sizes only |
| Fill | 綠 Green | `#00993E` | 93,2,100,0 | `--tdna-green` | white, display sizes only |
| Fill | 紅 Red | `#E4003D` | 0,100,67,0 | `--tdna-red` | white |
| Fill | 洋紅 Plum | `#C54090` | 23,86,0,0 | `--tdna-plum` | white |
| Action | 藍 Blue | `#004E9D` | 100,71,2,0 | `--tdna-blue` / `--accent` | white |
| Base | 淺灰 Grey | `#F6F6F6` | 0,0,0,5 | `--tdna-grey` / `--bg` | ink |
| Base | 近黑 Black | `#1E1F1C` | 75,65,65,80 | `--tdna-black` / `--fg` | white |

- **Semantic layer is what UI reads.** `--bg` paper grey, `--surface` white panels, `--fg` ink, `--fg-2` `#4A4C47` secondary copy and field labels, `--muted` `#66685F` captions and table heads, `--border` `#DCDDD8`, `--border-soft` `#ECEDE9`.
- `--accent` is CIS blue: primary buttons, links, selected nav, sort state, focus ring. One primary action per view.
- Status is only `--success` `#007A31`, `--warn` `#C4380C`, `--danger` `#C7002F` — CIS green, orange and red pressed darker so they pass 4.5:1 as text on white (5.5 / 5.4 / 6.1). As solid fills (badges, charts, posters) use the original CIS values. Never use the ten CIS colours as status colours.
- Tints for light backgrounds are always mixed from a CIS colour into `--surface`: `--tdna-tint-blue` 8% (organiser box, hint area), `--tdna-tint-green` 10% (Hub card bar, partner badge), `--tdna-tint-yellow` 25%, `--tdna-tint-pink` 50% (Hub card bars). Do not write new light hex values.
- `--surface-warm` is the pink tint; use it sparingly as a warm block, never as the page.
- Contrast (WCAG AA, measured): ink on yellow 11.3, cyan 7.0, pink 12.1, grey 15.3; white on blue 8.2, red 4.8, plum 4.7, black 16.6. Orange–white 4.0 and green–white 3.7 are display-size only; ink on orange 4.1 and green 4.4 are also display only. Blue takes white text, never ink. `--muted` on white 5.7, `--accent` on white 8.2.
- Dark mode exists for UI (`prefers-color-scheme: dark` and `data-theme="dark"`): surfaces `#141513` / `#1E1F1C`, text `#F1F1EC`, accent lifted to `#4F9BE8` with ink-blue text, status colours lifted. CIS fills keep their values; logos switch to the white files.

## Typography

| Use | Face | Weight | Token |
| --- | --- | --- | --- |
| Chinese, print and key visuals | TT Hei CHS Variable (licensed) | Extralight–Black | print only |
| English, print and key visuals | TT Commons Pro (licensed) | Light–ExtraBlack | print only |
| Chinese, web and UI | Noto Sans TC | 400 / 500 / 700 / 900 | `--font-body` chain |
| English and numerals, web and UI | Figtree | 400 / 500 / 600 / 700 / 800 | `--font-display`, `--font-body` |
| Code, kbd, tabular numbers | system monospace | — | `--font-mono` |

- The web pairing substitutes the licensed print faces with geometric sans of matching weight; do not swap in other faces or web-load the TT fonts without a licence.
- Scale: `--text-4xl` 40px display (public hero) · `--text-3xl` 30px / 800 KPI numbers · `--text-2xl` 26px / 800 page title, `--tracking-display` −0.01em · `--text-xl` 18px / 800 modal title · `--text-lg` 15px / 700 panel title · `--text-base` 14px body · `--text-sm` 13px secondary · `--text-xs` 12px labels only, 600, uppercase, `--tdna-tracking-label` 0.12em.
- Body `--leading-body` 1.5; headings `--leading-tight` 1.15 with `text-wrap: balance`. Numbers are `tabular-nums` everywhere.
- Chinese and English sit in the same text run without extra styling; the English wordmark is uppercase only inside lockups. Never letter-space Chinese body copy.
- Nothing visible below 12px; inputs are 16px on phones to avoid iOS zoom.

## Layout, edges and elevation

- 4px grid. Steps used: 4 / 8 / 12 / 16 / 24 / 32 (`--space-1/2/3/4/6/8`); component padding 12–16, block gap 24–32; `--space-12` 48 for section rhythm. Do not invent other values.
- Page shell: `--container-max` 1100px (admin console 1200px), white `--surface` panel on `--bg` paper, 1px `--border`, **left edge is the spine**: `--tdna-spine-width` 10px of `--tdna-spine` yellow. One spine per page or per card, never on both.
- Gutters 32 / 24 / 16px; section rhythm 64 / 48 / 32px. Phones drop the outer margin (`.page{margin:0}`) and keep the spine.
- **Radius is 0 everywhere.** Pills, avatars, chips and inputs are square-cornered.
- Elevation is a 1px ring (`--elev-ring`) or the hard offset shadow `--elev-raised` `4px 4px 0 var(--fg)` on hover of primary buttons and cards, paired with a 1px up-left translate. No blur, glass, glow, gradient or 3D.
- Focus: `--focus-ring` 2px accent ring outside a 2px surface gap on every focusable element.
- Mobile is a re-stack, never a squeeze: grids collapse to one column at 820–860px, tables scroll horizontally inside `.tbl`, nothing scrolls the page sideways.

## Logo and lockups

- Mark: `TDNA` in a structured slab serif — balance and stability from the letter construction, liveliness from the slab terminals. Files: `assets/logo/logo-black.svg`, `logo-white.svg`.
- Twelve fixed lockups, each in black and white SVG: `stacked-square`, `stacked-zh-en`, `stacked-zh`, `stacked-en`, `stacked-en2`, `horizontal-zh-en`, `horizontal-zh2-en2`, `horizontal-zh`, `horizontal-zh2`, `horizontal-en`, plus the type-only `wordmark-zh-en`. Distances between mark and wordmarks are calculated; **choose the lockup that fits the space, never re-assemble one.**
- Colour: black on white, light grey or light tints; white on CIS black or any solid CIS colour. No other colours, no gradients, no shadows, no outlines.
- Clear space: 50% of the mark height on all four sides for any lockup that contains the mark; wordmark-only lockups use the cap height of the `T`. Minimum: mark ≥ 24px tall in UI (favicon and nav may use the mark alone), horizontal lockups ≥ 120px wide.
- Do not: crop, change arrangement, use gradients, change proportions, apply effects, add shadows, change the wordmark typeface, outline.
- Auxiliary pattern: derived from the slab-serif strokes, geometric stroke ends counted in squares, colours interleaved in a rhythm; extends horizontally, mirrored left–right. The vector is not yet exported — take it from the VI 2.1 PDF chapter 5 or `TDNA Brand Assets.ai`; do not redraw it in CSS.

## Components

- **Primary button:** `--accent` fill, white text, 36px min height, 14px / 600, 0 radius; hover lifts with `--elev-raised` and a 1px translate; active drops to `--accent-active`. One per view. **Secondary:** white with `--border`; hover `--border-soft`. **Danger:** white with `--danger` text and border. **Small:** 32px, 12px text. Disabled: 50% opacity. 44px min height on phones.
- **Pill:** square 1px outline, 12px / 600, colour only from `good` / `warn` / `bad` / `brand` / `muted`.
- **KPI card:** `--surface`, 1px border, 12px tracked label, 30px / 800 value with a 13px unit, 12px `--fg-2` delta; `alert` variant colours border and value with `--warn`.
- **Panel:** header row (15px / 700 title + 12px muted meta) with a `--border-soft` rule, 16px body.
- **Hub card:** white card whose left bar is one CIS colour (yellow / cyan / pink / green) via `--card-bar`; 12px uppercase date line, 15px title, 13px place, one pill; hover uses `--elev-raised`. Bars rotate between cards; they never encode status.
- **Tint box:** organiser, partner, reminder and price boxes on `--tdna-tint-*` with a 1px border.
- **Form:** 12px / 600 `--fg-2` labels above 36px inputs with a `--tdna-ctrl` `#8A8C86` border (≥3:1), focus ring `--focus-ring`; errors turn the border and a 13px message `--danger`, never colour alone; two-column grid collapsing to one.
- **Table:** 12px uppercase muted heads, sortable head in `--accent`, 10×12px cells, `--border-soft` row rules, hover row at 6% accent, numbers right-aligned tabular; wrap in `.tbl` for horizontal scroll.
- **Note:** dashed `--border` box, 13px `--fg-2`. **Toast:** ink background, paper text, 600.
- **Nav:** top bar (public) or 232px sidebar (admin) with the spine; links `--fg-2` / 600, active link `--accent` with a 3px accent underline or left bar.
- **Footer:** 12px muted line with the horizontal English lockup at 20px.

## Motion

- `--motion-fast` 120ms for hover colour, `--motion-base` 150ms for shadow and translate; `--ease-standard` ease-out. Nothing longer than 250ms; no bounce, parallax, float or autoplay.
- Only background, box-shadow, color and a 1px transform animate. Respect `prefers-reduced-motion` by removing all transitions.

## Applications

- Instagram posts 1080×1350 with the eight-category colour system in `tdna://ig/guide`; white lockup on a solid CIS colour, headline in Noto Sans TC 900 / Figtree 800.
- Decks 16:9: white slides, spine on the left edge of title slides, one CIS colour per section divider; titles ≥ 32px, body ≥ 20px at 1920×1080.
- Documents and government correspondence: black horizontal `zh-en` lockup top-left, Noto Sans TC body 12pt, no colour blocks.
- Print: CMYK values from the table, 300dpi, 3mm bleed, outlined text; business card 90×54mm master in `TDNA-namecard-90x54.pdf`.
- Co-branding: TDNA lockup separated from partner marks by clear space ≥ the mark height; partners' marks used as supplied.

## Do's and don'ts

- **Do** read colours through the semantic tokens and keep the ten CIS values untouched.
- **Do** keep one spine, square corners and hard shadows — that is the whole "TDNA feel".
- **Do** use the provided lockups and Taiwan wording.
- **Don't** add gradients, rounded corners, blur shadows, glass, glow or new colours.
- **Don't** use CIS green/red as small text, or CIS colours as status.
- **Don't** redraw, recolour, stretch or re-combine the mark; don't borrow TDF's pixel type or black grid.
