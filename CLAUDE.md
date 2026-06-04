# GAME Lab Website — Project Context

## Site
- Live at https://gamelab-bio.github.io
- Jekyll + minima theme, hosted on GitHub Pages
- Repo: https://github.com/gamelab-bio/gamelab-bio.github.io.git

## Current State
- Placeholder content (people, research, publications, news) is intentional — real content not ready until ~August 2026. Do not suggest filling it in.
- Entry page (`index.html`) is an interactive puzzle gate with 5 mini-games; visitors solve it to enter the site.
- Logo (`assets/images/logo.svg`) is displayed full-width on the main page (`about.md`), not in the header.
- A "solve the entry puzzle again" link sits at the bottom of `about.md` linking back to `/`.

## Git
- Push via HTTPS using a PAT stored in the remote URL.
- Two GitHub accounts in use: personal (Vivaldi browser) and gamelab (Chrome browser). Always push as the gamelab account.

## Stack
- `index.html` — standalone puzzle entry page (no Jekyll layout)
- `_includes/header.html` — nav only, no logo
- `_sass/custom.scss` — all custom styles
- `about.md` — main/landing page
- `_config.yml` — Jekyll config, header_pages order
