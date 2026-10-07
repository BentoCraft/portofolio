# Agus Juniartha — Portfolio

Portfolio site built with [Astro](https://astro.build) (static output). Two pages: `/` (home) and `/wine-adore/` (case study).

## Develop
```bash
npm install
npm run dev       # http://localhost:4321
npm run build     # output in dist/
npm run preview   # serve the production build
```

## Structure
- `src/pages/index.astro`, `src/pages/wine-adore.astro` — the pages
- `src/layouts/Base.astro` — head, meta, fonts
- `src/styles/global.css` — design tokens (light/dark) and responsive rules
- `design-system/` — brand book and component previews; `design/` — original design sources
- `legacy/index.html` — the original single-file site, kept for reference

## Deploy
Hosted on Vercel (framework preset: Astro, build `npm run build`, output `dist`).
