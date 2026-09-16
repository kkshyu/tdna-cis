# TDNA Usage

Package guide for OpenDesign agents building Taiwan Digital Nomad Association (TDNA) artifacts: admin console pages, Hub public pages, event posts, decks, documents and print.

## Read Order

1. Read this file for the package contract.
2. Read `DESIGN.md` for the VI 2.1 rules: mark and lockups, the ten CIS colours, type pairing, spine, edges, components and hard prohibitions.
3. Paste the whole `:root` block from `tokens.css` into the first `<style>` of the artifact before writing any component CSS. Copy the two dark-mode blocks too if the artifact is a UI that people will open at night; leave them out for print and social images.
4. Load fonts from Google Fonts: `Figtree` (400–800) and `Noto Sans TC` (400/500/700/900). Print and key visuals use the licensed TT Hei CHS Variable / TT Commons Pro — do not substitute those with other faces on the web; Figtree + Noto Sans TC is the only approved web pairing.
5. Reuse the recipes in `components.html` (spine page shell, hero, buttons, pills, KPI cards, panel, tint cards, form, table, note, toast, footer) before inventing new controls.
6. Pick the logo lockup from `assets/logo/` that fits the space (`logo-*`, `stacked-*`, `horizontal-*`, `wordmark-*`; each in `black` and `white`). Never assemble a lockup yourself.
7. `assets/pattern.svg` is the auxiliary pattern (four densities, eight CIS colours): use one row as a divider or edge band, scaled proportionally, never rearranged.
8. Open `preview/` pages for a visual sanity check of colours, type scale, spacing, logos and components.

## Design Highlights

- Visual style: calm editorial grid, white panels on light-grey paper, one 10px yellow spine on the left edge, square corners, hard 4px offset ink shadow on hover.
- Colour stance: ten CIS colours used as fills exactly as specified; UI reads only the semantic layer (`--accent` blue, `--success` / `--warn` / `--danger` pressed darker for text contrast, four `--tdna-tint-*` backgrounds mixed from CIS colours).
- Type: Figtree for Latin and numerals, Noto Sans TC for Traditional Chinese, 14px body, 12px uppercase tracked labels, 26px / 800 page titles. Taiwan wording in Chinese.
- Mark: slab-serif `TDNA`, structured and stable; twelve fixed lockups, black or white only, clear space = 50% of mark height.

## Do

- Keep every schema token name intact; add brand values only through the `--tdna-*` extensions.
- Use `--accent` (CIS blue) for the one primary action, links and selected states; secondary buttons are white with a `--border` outline.
- Keep the spine (`--tdna-spine-width` of `--tdna-spine`) on the left edge of the page shell or a card, once per page.
- Use the tints (`--tdna-tint-blue/green/yellow/pink`) for Hub card bars, organiser boxes and hint areas; never write new hex values for light backgrounds.
- Keep body text at 14px or larger and labels at 12px with `--tdna-tracking-label`; every text/background pair must meet 4.5:1 (see the AA table in `DESIGN.md`).
- Show the logo from the SVG files unchanged, on white, light grey, CIS black or a solid CIS colour (white version on colour).

## Avoid

- No rounded corners, gradients, blur shadows, glass, glow or 3D — radius tokens are 0 and `--elev-raised` is a hard offset on purpose.
- No new colours; the ten CIS colours plus the derived semantic layer and tints are the entire palette.
- Never use CIS green `#00993E` or red `#E4003D` as small text on white — use `--success` / `--danger`.
- Never treat the ten CIS colours as status colours; status is only `--success` / `--warn` / `--danger` / `--accent`.
- Never crop, recolour, stretch, outline, shadow, gradient or re-combine the mark and wordmarks; never redraw the mark in type.
- No Simplified Chinese characters or mainland terms; write in Taiwan Traditional Chinese.
