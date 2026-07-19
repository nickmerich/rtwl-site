# Run Takoma With Love — The Story

Event story site for the Run Takoma With Love 5K (Sunday, August 2, 2026 · Takoma-Piney Branch Local Park, Takoma Park, MD). Built in the GRYT Club / grytrun.com design language.

## Stack

Zero-dependency static site — plain HTML, CSS, and vanilla JS. No build step required. A Vite config is included only for convenience (`npm run dev`), so it also opens cleanly in AI builders.

- `index.html` — all content and interaction JS (reveal animations, countdown, scrollspy, copy-invite, sticky register bar)
- `styles.css` — full design system (see design tokens below)
- `assets/` — flyer + photography (webp)
- `rtwl.ics` — add-to-calendar file linked from the hero
- `favicon.svg`

## Import into Lovable

1. Push this folder to a GitHub repo (or upload the zip contents to a new repo).
2. In Lovable: **Create project → Import from GitHub** and select the repo.
3. Lovable will run it with Vite (`npm install && npm run dev`). The site is the root `index.html`.
4. Prompting tip: tell Lovable "this is a static HTML/CSS site — keep the design tokens in `styles.css` `:root` untouched" so iterations stay on-brand.

Note: if you later use `vite build`, move `rtwl.ics` into a `public/` folder so it ships to `dist/` (plain `<a href>` files aren't auto-bundled).

## Design tokens (match grytrun.com)

- `--paper: oklch(0.972 0.012 85)` warm paper background
- `--green: oklch(0.34 0.045 165)` Takoma green (headers, badges)
- `--rust: oklch(0.6 0.15 32)` love rust (event name, CTAs, hearts)
- `--water: oklch(0.55 0.11 245)` smartwater blue — hydration accent ONLY
- Fonts: Bebas Neue (display) · Caveat Brush (script) · Playfair Display italic (pull quotes) · Inter (body)
- Torn-edge treatment: `--torn` clip-path on buttons, badges, cards

## Content guardrails (keep these true)

- Event name is **Run Takoma With Love**; *From Takoma With Love* is the album (Oddisee and Heno., Outer Note). They are not a duo — never describe them as one.
- No artist performance/appearance promises.
- Permit-facing scope (per permit packet): free RSVP, capped at 100, no vendors, no admission fees, no merchandise sales, no amplified sound, on foot only, no road closures or shuttles, nothing staged in residential areas.
- Official public timeline: check-in 8:30, welcome + safety 9:00, walk/run begins **9:15**, return + hydration 10:30, community connection 10:50, park gathering 11:30, light refreshments (pre-packaged, if permitted) 12:15, closing 12:45, site cleared by 2:00.
- Water: primary station at the shelter (smartwater in-kind). A second route stop exists ONLY if approved — keep "if approved" language until confirmed. No residential placement.
- No grill/cookout, no field-day games, no Ed Wilhelm Field use — do not reintroduce this language.
- Route: from the park out to the open (car-free) parkway and back; volunteer marshals along the route with two marshaled road crossings; ADA parking/routes stay clear.
- Permit is under M-NCPPC review — do not launch publicly until written approval.
- Course map is a sketch, not to scale; official map goes out in the runner email.

## Local dev

Open `index.html` directly, or:

```bash
npm install && npm run dev
```
