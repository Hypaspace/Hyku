# Hypaspace — Streets of Growth Brand System

## Project Overview
Static HTML/CSS/JS brand design system documentation site for Streets of Growth (SOG).
Hosted on GitHub Pages via the `brandsystem` repo (`git@github.com:streetsofgrowth/brandsystem.git`).

## Stack
- Vanilla HTML5 / CSS3 / JavaScript (no framework, no build tools, no npm)
- Chart.js (CDN) for data visualizations
- Material Icons (CDN)
- 127+ custom SVG icons in /icons/

## Structure
- `index.html` — single-page brand documentation site (all content, styles, and scripts inline)
- `icons/` — 127+ custom SVG icon files

## Design Tokens (CSS Custom Properties)
- Primary: SOG Purple `#625D9C`
- Blue `#4197CB`, Sky `#5EB3E4`, Teal `#0095A9`, Green `#00AF9A`
- Charcoal `#323E48`
- Red `#F32735`, Orange `#FF6C0E`, Yellow `#F2CD00`
- Off-white `#F5F5F7`

## Conventions
- All styling via CSS custom properties (no preprocessors)
- Dark floating sidebar: gradient from `#2C2A46` to `#00434C`, white logo
- No build step — edit `index.html` directly, changes are immediate
- Icons are standalone SVG files referenced in `index.html`
- No TypeScript, no linting, no testing framework

## Deployment
Push to `main` branch → GitHub Pages auto-deploys.
