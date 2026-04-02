# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Website for **DDr. Michael Antolini** — a veterinary practice (Tierarzt) in a historic villa in Vienna-Hietzing (1130 Wien, Seelosgasse 20). The site targets affluent, cultured pet owners in Vienna.

## Architecture

- **Static HTML site** hosted on Netlify (no build step, no static site generator)
- **Decap CMS** (formerly Netlify CMS) at `/admin/` for content management via Netlify Identity + Git Gateway
- **Domain:** tierarztantolini.at (DNS at one.com, hosting on Netlify)
- **GitHub:** github.com/tierarztwien/tierarztwien

## Key Files

- `index.html` — The entire website (single-page, all CSS/JS inline)
- `impressum.html` — Legal imprint (ECG § 5, Austrian law)
- `datenschutz.html` — Privacy policy (DSGVO/GDPR Art. 13)
- `admin/index.html` — CMS admin panel entry point
- `admin/config.yml` — Decap CMS collections and field definitions
- `netlify.toml` — Netlify config (headers, redirects)
- `robots.txt` — Search engine directives

## Design System (Villa Classica)

- **Palette:** Cream `#faf8f4`, Brown `#2d2926`, Gold `#8b7355`, Gold-pale `#d4c5a9`, Warm-white `#fff9f0`
- **Fonts:** Cormorant Garamond (serif, headings), Montserrat (sans, body) — hosted locally in `/fonts/` (DSGVO requirement, no Google Fonts CDN)
- **Tone:** Warm, elegant, Italian heritage, personal care

## DSGVO/Privacy Constraints

- **No external font loading** — all fonts must be local (`/fonts/`)
- **Google Maps** uses 2-click solution — only loads after explicit user consent
- **No tracking scripts** — no Google Analytics, no Facebook Pixel, no third-party cookies
- **Cookie banner** appears immediately (no delay), with granular consent options
- **All images** must be served locally, not from external CDNs
- When adding new external resources: always check DSGVO compliance first

## Deployment

Changes pushed to `main` branch auto-deploy to Netlify within ~30 seconds. No build command needed.

```bash
git add <files>
git commit -m "description"
git push origin main
```

## Content & Images

- Images with SEO-optimized filenames in `/images/` (e.g., `tierarzt-antolini-mit-hund-wien.jpg`)
- Original photos in `/Fotos/` (source files, not deployed directly)
- CMS content in `/content/` (galerie, bewertungen, leistungen, instagram, settings)
- CMS is set up but NOT connected to index.html — content changes require manual HTML edits for now

## Language

All website content, commits, and documentation should be in **German (Austrian)** unless specified otherwise.
