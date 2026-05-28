# AGENTS.md

## What this is

A static Reveal.js presentation (Bahasa Indonesia) describing the Unit Head QC role at PT Mayora. Single-page slide deck.

## Stack

- **Framework:** [Reveal.js](https://revealjs.com/) (vended at `assets/reveal/`)
- **Custom CSS:** `assets/css/ptc.css`, fonts at `assets/css/fonts.css`
- **Fonts:** Exo 2, Orbitron, Share Tech Mono, Michroma (local woff2 in `assets/fonts/`)
- **Icons:** Font Awesome 6 (local in `assets/webfonts/`)
- **Reference doc:** `PTC UH.pdf` at repo root

## Commands

No build step exists. Serve with any static server:

```sh
# Python
python3 -m http.server 8000

# npx
npx serve .
```

## Structure

- `index.html` — all slide content inline
- `assets/css/ptc.css` — theme, layout, component styles
- `assets/reveal/` — vendored Reveal.js (do not modify directly)
- `assets/img/` — images (`logo.webp`, `login-bg.jpg`, etc.)
- `assets/icon/` — PWA favicons + `site.webmanifest`

## Conventions

- All text is in Indonesian (id)
- Slide transitions: `fade`, speed `fast`
- Slide dimensions: 1366×768, margin 0.04
- No package.json, no CI, no tests
