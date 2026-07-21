# Hypaspace

## Overview
This folder is the **Hypaspace** brand umbrella and the Hyku website's git repo
(`git@github-hypaspace:Hypaspace/Hyku.git`, branch `main`, domain `hyku.co.uk`).

Products created under the Hypaspace brand live here:
- Hyku website — the tracked files at the repo **root** (see below)
- `HYBRIJ/` — public release macOS app (untracked / local)
- `HYBRIJ Lite/` — friend's lightweight version of HYBRIJ (untracked / local)
- `Hylift/` — audio-extractor macOS app (untracked / local; has its own `CLAUDE.md`)

## Hyku website (repo root)
- `index.html` — "HYKU — System Initialisation" boot/intro screen; ENTER navigates to `main.html`
- `main.html` — "HYKU — Synthesising Code & Craft" main single-page site (nav, skills, connectors, footer)
- `CNAME` — custom domain (`hyku.co.uk`)
- `README.md`

**hyku.co.uk serves from these repo-ROOT files** — keep `index.html` / `main.html` at the root.

### Web stack
- Vanilla HTML5 / CSS3 / JavaScript (no framework, no build tools, no npm)
- Google Fonts via CDN — JetBrains Mono (`index.html`); Share Tech Mono + Rajdhani (`main.html`)
- Google Material Symbols (CDN)
- No build step — edit the HTML directly; all styling inline via CSS custom properties
- No TypeScript, no linting, no testing framework

## macOS apps
Each app subfolder is a standalone Xcode project with `build.sh` / `distribute.sh` scripts, and is
local-only (not tracked in this repo). After any public-HYBRIJ code change, end with the DMG build
command (build via `HYBRIJ/build.sh` / `distribute.sh`).

## Deployment
Push to `main` → GitHub Pages "deploy from branch" auto-deploys the root `index.html` / `main.html`.
Live update lands ~2-3 min later (CDN `max-age=600`), so hard-refresh when checking.
