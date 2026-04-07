# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Community website for The Sensemaking Scenius. Plain HTML/CSS static site deployed to GitHub Pages at **www.scenius.space**.

Rebuilt from the original [mmm.page](https://kpaxle.mmm.page/scenius) as an open-source, community-editable project. The goal is faithful reproduction of the original whimsical, storytelling-driven design.

## Architecture

```
site/                  → Deployed directory (GitHub Pages serves this)
  index.html           → Main narrative scroll page
  about.html           → Mission, principles, backstory
  styles.css           → All styles (shared across pages)
  assets/images/       → GIFs, PNGs, decorative elements
  CNAME                → Custom domain (www.scenius.space)
raw_ressources/        → Original mmm.page HTML export (gitignored, reference only)
vibecoded-landing/     → Workshop landing page experiment (gitignored, local only)
```

No build step, no framework, no dependencies. Push to `main` → GitHub Actions deploys `site/` automatically.

## Deployment

Push to `main` triggers `.github/workflows/deploy.yml` which deploys the `site/` directory to GitHub Pages via `actions/deploy-pages@v4`.

## Design Reference

The original site is at [kpaxle.mmm.page/scenius](https://kpaxle.mmm.page/scenius) (main) and [kpaxle.mmm.page/scenius-about](https://kpaxle.mmm.page/scenius-about) (about). Use these as the visual reference for CSS work.

Key design elements:
- **Background:** teal/mint (`rgb(129, 215, 192)`)
- **Fonts:** Calistoga (display), Rubik Glitch (glitch text), EB Garamond (body), Lato (sans)
- **Layout:** Freeform narrative scroll with absolutely-positioned decorative GIFs and shapes
- **About page:** Uses dark text (`#2a2a2a`) on teal, not white text

## Known Issues

The GIF mapping is wrong — the clone reuses `giphy.gif` for most positions but the original uses distinct GIFs at each location. The "spirals" section uses SVG paths but the original uses spinning GIF instances. See [issue #1](https://github.com/sensemaking-scenius/scenius-website/issues/1) for full details.

## Community Context

This is a community project — changes go through PRs. The community reviews changes via preview URLs shared in Telegram. Workshop decisions and roadmap are documented in the [Notion page](https://www.notion.so/m4co/Website-Workshop-30596ae9065580dda873d6b2120a6eef) and GitHub issues.

GitHub org: `sensemaking-scenius`. Repo was renamed from `website-ressource` to `scenius-website` — old URLs redirect.
