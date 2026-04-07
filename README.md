# The Sensemaking Scenius Website

The community website for The Sensemaking Scenius — a community of practice for digital builders, researchers, artists & activists who share a vision of a regenerative, intentional & meaningful internet.

**Live:** https://www.scenius.space/

## Background

The original website was built by Kristen on [mmm.page](https://mmm.page). In our [Feb 12, 2026 workshop](https://www.notion.so/m4co/Website-Workshop-30596ae9065580dda873d6b2120a6eef), the community agreed to rebuild it as an open-source project so that anyone can contribute via pull requests.

This repo is that rebuild. Alexandre downloaded the original HTML and used Claude to reconstruct clean CSS/HTML — that's the `raw_ressources/` (original export) and `site/` (clean reconstruction) directories. Jon then structured it for GitHub Pages deployment.

## Structure

```
site/
  index.html          # Main page (narrative scroll)
  about.html           # Mission, principles, backstory
  styles.css           # All styles
  assets/images/       # GIFs, PNGs, decorations
raw_ressources/        # Original mmm.page HTML export (reference only)
.github/workflows/
  deploy.yml           # Auto-deploys site/ to GitHub Pages on push
```

Plain HTML/CSS — no build step required. Edit the files, push, and GitHub Pages deploys automatically.

**Hosting:** Currently on GitHub Pages (free for public repos). [Netlify's open-source program](https://www.netlify.com/legal/open-source-policy/) is an alternative if we need more features.

## Contributing

1. Fork the repo
2. Make your changes in the `site/` directory
3. Open a pull request

You can also use GitHub's web editor (click the pencil icon on any file) for quick changes without cloning.

For larger changes, Claude Code or any LLM can help — just point it at the repo and describe what you want.

## Roadmap

Based on the [Feb 12, 2026 workshop](https://www.notion.so/m4co/Website-Workshop-30596ae9065580dda873d6b2120a6eef) decisions. Issues track all planned work.

### V1 — Faithful Reproduction (current)

Migrate the existing mmm.page site into a community-editable, open-source format.

- [x] Reconstruct main page as HTML/CSS (Alexandre + Jon)
- [x] Deploy to GitHub Pages
- [x] Create about page (mission, principles, backstory)
- [ ] [CSS polish: visual comparison pass](https://github.com/sensemaking-scenius/website-ressource/issues/1)
- [ ] [Migrate to 11ty](https://github.com/sensemaking-scenius/website-ressource/issues/2)
- [ ] [Contributor guide](https://github.com/sensemaking-scenius/website-ressource/issues/8)
- [ ] [PR preview deployments + Telegram approval flow](https://github.com/sensemaking-scenius/website-ressource/issues/13)

### V2 — Brand Upgrade

Apply the Scenius brand identity and integrate content feeds. Preserve the storytelling narrative flow while giving it a cohesive visual identity.

- [ ] [Apply Scenius brand (Spencer's design)](https://github.com/sensemaking-scenius/website-ressource/issues/3)
- [ ] [Integrate Paragraph blog](https://github.com/sensemaking-scenius/website-ressource/issues/4)
- [ ] Easter eggs and personality (raccoons!)

### V3 — Subpages as Needed

Each member can pilot their own subpage linked from the main page — they can look different and be their own thing ("multi-perspectival").

- [ ] [Professional subpage for funders/grants](https://github.com/sensemaking-scenius/website-ressource/issues/5)
- [ ] [Project subpages](https://github.com/sensemaking-scenius/website-ressource/issues/6)
- [ ] [Member directory](https://github.com/sensemaking-scenius/website-ressource/issues/7)
- [ ] [Surface Knowledge Graph content](https://github.com/sensemaking-scenius/website-ressource/issues/11)
- [ ] [Integrate Portico co-presence app](https://github.com/sensemaking-scenius/website-ressource/issues/12)

## Domain

Custom domain **www.scenius.space** is live and pointing at this repo's GitHub Pages deployment.

## Design Inspiration

Sites we referenced during the workshop:

- [metagov.org](https://metagov.org/) — clean, multiple perspectives on the same org
- [mosaic-labs.org](https://mosaic-labs.org/) — clean and simple
- [oatly.com](https://www.oatly.com/en-us) — playful brand storytelling
- [panic.com](https://panic.com/) — personality-driven
- [duolingo.com](https://www.duolingo.com/) — fun, character-driven
- [cardsagainsthumanity.com](https://www.cardsagainsthumanity.com/) — irreverent
- [dirt.fyi](https://dirt.fyi/) — indie publication aesthetic
- [100r.co](https://100r.co/site/home.html) — minimal, handcrafted
- [maggieappleton.com](https://maggieappleton.com/) — digital garden / knowledge-oriented

## License

This is a community project of The Sensemaking Scenius.
