# How AI Agents Built This Page

## Overview

This "Selected Works" page was created through a collaborative process between Bernhard Mueller and AI coding agents (Claude Code). The workflow demonstrates how AI agents can assist with research compilation, web design, and content creation.

## Workflow

### Phase 1: Research Compilation

AI agents were used to systematically gather Bernhard's published works across multiple sources:

- **GitHub repositories** — crawled public repos for star counts, descriptions, and links
- **SEC Consult vulnerability lab** — compiled advisories from the 2005-2013 era
- **Exploit-DB / PacketStorm** — cross-referenced vulnerability disclosures
- **Medium articles** — catalogued technical writing across multiple publications (HackerNoon, ConsenSys, personal blog)
- **Conference materials** — located papers, slides, and talk videos from HITB, DEF CON, and other venues
- **arXiv** — found the Hound research paper

The compiled data lives in `resources/works.md` as the canonical source of truth.

### Phase 2: Page Design & Implementation

The page was designed and built as static HTML with:

- A **timeline-based layout** that tells the career story chronologically
- **Paper excerpt blocks** that highlight key ideas from each major work
- **Talk/video cards** with prominent play buttons for conference presentations
- **Reveal-on-scroll animations** using IntersectionObserver
- Consistent use of the Floating Pragma design system (JetBrains Mono, dark theme, accent colors)

### Phase 3: Deployment

The page deploys automatically via GitHub Actions to GitHub Pages whenever changes are pushed to the `main` branch.

## What the Agents Did vs. Didn't Do

**Agents handled:**
- Searching across GitHub, Medium, SEC Consult, Exploit-DB, and conference archives
- Compiling and cross-referencing findings into structured markdown
- Generating the HTML/CSS/JS for the page
- Writing representative excerpt text based on paper descriptions
- Creating deployment configuration

**Human handled:**
- Reviewing compiled works for accuracy and completeness
- Creative direction and feedback on layout
- Final approval of all content
- Publishing decisions

## Tools Used

- **Claude Code** (Anthropic) — primary AI coding agent
- **GitHub Pages** — hosting
- **GitHub Actions** — CI/CD

## Project Context

This is one of several properties under the [Floating Pragma](https://floatingpragma.io) umbrella:

| Property | Description |
|----------|-------------|
| [floatingpragma.io](https://floatingpragma.io) | Landing page |
| [STARK Lab](https://floatingpragma.io/starklab/) | Interactive STARK proof tutorial |
| [Awesome ZK Proofs](https://floatingpragma.io/awesome-zk-proofs/) | ZK learning path |
| [Awesome AI Security](https://floatingpragma.io/awesome-ai-security/) | AI security learning path |
| **Selected Works** | This page — career portfolio |
