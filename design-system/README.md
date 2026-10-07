# Agus Juniartha — Personal

A light, minimal system for the personal portfolio of I Wayan Agus Juniartha, Flutter mobile developer from Bali. Quiet off-white ground, near-black type, and one confident blue borrowed from the Flutter world. The work is the colour; the system stays out of its way.

## Content fundamentals

- **Voice:** first person, direct, concrete. "I build Flutter apps for iOS and Android." not "Passionate innovator crafting experiences."
- **Show, don't claim:** name the thing shipped (payment gateway, push notifications, Play Store releases) instead of adjectives.
- **Short:** headings ≤ 6 words, bullets one line where possible, About ≤ 80 words.
- **Dates** in mono label style, uppercase: `JUL 2024 — PRESENT`.
- **No invented numbers.** Unknowns are written `[PLACEHOLDER]` until real.

## Visual foundations

**Colour.** `surface` is the page; `surface-raised` lifts cards and the nav; `surface-sunken` bands alternate sections. Text is `ink`, secondary text `ink-muted`. `accent` is the only hue — use it for primary buttons, links, the active nav item and at most one highlight per section. `accent-soft` fills skill chips. Hairlines use `line`; anything a user must see as a control edge uses `line-strong`.

**Type.** Space Grotesk (`display`) for headings, IBM Plex Sans (`body`) for reading, JetBrains Mono (`mono`) for labels, dates and chips — a quiet nod to code. Load all three from Google Fonts:
`https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600&family=IBM+Plex+Sans:wght@400;500&family=JetBrains+Mono:wght@500&display=swap`

**Space & grid.** 12-column grid inside `container-max` (1120px), 24px gutters (`space-4`), `space-6` side margins. Sections are separated by `space-7` on desktop, `space-6` on phone. Generous whitespace beats boxes.

**Shape.** `radius-sm` for buttons, `radius-md` for cards, `radius-pill` for chips. Borders not shadows: cards use a 1px `line` border; no drop shadows, no gradients.

**Motion.** Minimal: 150ms ease-out colour/underline changes on hover. Nothing bounces.

## Iconography

Thin 1.5px stroke icons, 20px, `currentColor`, round caps (Lucide-style). Only where they aid scanning: contact links, external-link arrows, store badges. No emoji, no illustrations.

## Components

- **Button** — primary (accent fill) and ghost (line-strong border).
- **Chip** — skill / stack tag in mono on `accent-soft`.
- **NavBar** — name wordmark left, anchor links right, one CTA.
- **SectionHeader** — mono number + h2 + optional lead.
- **ExperienceRow** — date column + role, company, bullets.
- **ProjectCard** — image frame, title, one-line summary, chips.

## Accessibility

All text pairs meet 4.5:1 in both themes (`ink-muted` on `surface` ≈ 7:1). Touch targets ≥ 44px. Visible focus ring in `focus`. Real `<a>` and `<button>` elements only.
