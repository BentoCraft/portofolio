# Agus Juniartha — portfolio site

Personal portfolio for I Wayan Agus Juniartha, Flutter mobile developer in Bali.

## Files
- `index.html` — the whole live site: one self-contained page, no build step. Two views in one file:
  - `#view-home` (home page) and `#view-case` (Wine Adore case study, opened with `#wine-adore`).
  - A small script at the bottom switches views on `hashchange` and runs the phone menu button.
- `design-system/` — the design system the site follows (`tokens.json`, `README.md` brand book, component previews). Read `design-system/README.md` before changing the look.
- `design/` — the original design-canvas sources (`.dc.html`), kept for reference only. Edit `index.html`, not these.

## Rules for edits
- Colors: only use the CSS variables defined in `:root` at the top of `index.html` (`--surface`, `--raised`, `--sunken`, `--ink`, `--muted`, `--line`, `--line-strong`, `--accent`, `--accent-soft`, `--on-accent`, `--inverse*`). Every variable has a light value and a dark value; add new colors to all three blocks (`:root`, the `prefers-color-scheme: dark` block, and `[data-theme="dark"]`).
- Fonts: Space Grotesk (headings), IBM Plex Sans (body), JetBrains Mono (labels, dates, chips), loaded from Google Fonts.
- One accent color only (blue). Borders, not shadows. Radius 6px buttons, 12px cards, pill chips.
- Responsive rules live in the `@container (max-width: 720px)` block; the page must work at 390px wide.
- No invented facts or numbers. Unknowns stay as `[PLACEHOLDER]` text.

## Content still missing
- Profile photo (replace the "AJ" circle in the hero profile card).
- App Store / Google Play links and screenshots on the Wine Adore case study.
- A real metric for the case study "Outcome" section, if available.

## Run locally
Open `index.html` in a browser, or serve the folder: `npx serve .` (or `python3 -m http.server`).
