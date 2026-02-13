# Selected Works — Bernhard Mueller

## What This Is

A curated portfolio of 20+ years of offensive security research, tools, talks, papers, and vulnerability advisories by Bernhard Mueller. Part of the [Floating Pragma](https://floatingpragma.io) web presence.

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

Follows the shared Floating Pragma design tokens:

- **Background**: #0a0a0a / #111111 / #1a1a1a
- **Accents**: green #00ff41, purple #ff79c6, cyan #4ee7ff, amber #ffb300, rose #f43f5e, blue #60a5fa
- **Font**: JetBrains Mono
- **Effects**: scan-line animation, glow, card hover translateY(-2px), reveal-on-scroll

## Key Design Decisions

- **Timeline layout** with a gradient vertical line connecting eras (blue → green → purple → cyan → amber → rose)
- **Paper excerpts** styled as terminal-like blockquotes with `>` prompt character and source attribution
- **Talk/video cards** with play button indicators for conference presentations
- **Era-based navigation** with sticky pills and IntersectionObserver highlighting
- **Stats ribbon** in the hero showing career metrics at a glance
- Each era has its own accent color for visual distinction

## Content Eras

| Era | Color | Period | Org |
|-----|-------|--------|-----|
| Early Security Research | Blue | 2005-2013 | SEC Consult |
| Mobile Security | Green | 2014-2018 | Vantage Point / OWASP |
| Smart Contract Security | Purple | 2017-2020 | ConsenSys Diligence |
| AI & Autonomous Agents | Cyan | 2023-Present | Sherlock |
| Writings | Amber | Ongoing | Medium |
| Theoretical Physics | Rose | Side Quest | Independent |
| Learning Platforms | Amber | 2025-Present | floatingpragma.io |

## Important Notes

- This repo must NOT have a CNAME file (only the root `muellerberndt.github.io` repo has one)
- Google Analytics ID: G-HLGH209WMG (shared across all floatingpragma.io properties)
- The `resources/works.md` is marked DRAFT — verify any additions against primary sources
- All paper excerpts in the HTML are paraphrased/representative, not verbatim quotes
