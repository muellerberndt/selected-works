# Selected Works — Bernhard Mueller

## What This Is

A curated portfolio of 20+ years of offensive security research, tools, talks, papers, and vulnerability advisories by Bernhard Mueller. Part of the [Floating Pragma](https://floatingpragma.io) web presence.

The live CV is https://floatingpragma.io/work/ (repo `muellerberndt.github.io`, file `work/index.html`,
styled by the site's `assets/stealth.css`). `web/index.html` in this repo is a redirect stub to it.
`resources/` keeps the research notes the CV was compiled from.

## Architecture

- **Static HTML** — single `web/index.html` file, no build step
- **Deployed** via GitHub Pages (`gh-pages` branch) using GitHub Actions
- **URL**: https://floatingpragma.io/selected-works/
- **Source data**: `resources/works.md` — the raw research compilation (canonical source of truth for all works)

## Directory Structure

```
selected-works/
├── CLAUDE.md              # This file
├── AGENTS.md              # How AI agents were used to build this
├── README.md              # Repo description
├── resources/
│   ├── works.md           # Raw compiled works data (source of truth)
│   └── packetstorm-1.txt  # PacketStorm archive data
├── web/
│   ├── index.html         # The actual page (static HTML + CSS + JS)
│   ├── sitemap.xml
│   ├── robots.txt
│   └── favicon.svg
└── .github/
    └── workflows/
        └── deploy.yml     # GitHub Pages deployment
```

## Design System

All floatingpragma.io pages share the landing page's theme: black background, cyan `#4af1f2` glow,
system monospace stack, the pixel caret logo, scanlines. The stub here uses the same colours.

## Important Notes

- This repo must NOT have a CNAME file (only the root `muellerberndt.github.io` repo has one)
- Google Analytics ID: G-HLGH209WMG (shared across all floatingpragma.io properties)
- The `resources/works.md` is marked DRAFT — verify any additions against primary sources
- All paper excerpts in the HTML are paraphrased/representative, not verbatim quotes
