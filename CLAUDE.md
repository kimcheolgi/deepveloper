# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static portfolio/landing page for "Deepveloper" — a personal hub showcasing zero-cost web services hosted on Vercel. The entire site is a single HTML file with embedded CSS and JavaScript.

## Files

- `deepveloper-index.html` — The entire site (HTML, CSS, JS all in one file)
- `deepveloper-CNAME` — Domain: `blog.deepveloper.com`

## Development

No build step, dependencies, or tooling. Open `deepveloper-index.html` directly in a browser to preview. To serve locally:

```bash
npx serve .
# or
python3 -m http.server 8080
```

## Architecture

Single-file static page. All styles are in a `<style>` block and all scripts are in a `<script>` block at the bottom of the HTML.

**Design tokens** (defined as CSS custom properties in `:root`):
- Background: `#0A0A0F`, Text: `#E4E4E7`
- Accent: `#6366F1` (indigo), `#10B981` (emerald)
- Fonts: "Outfit" (body), "JetBrains Mono" (code)

**JavaScript behavior:**
- Scroll-triggered navbar styling
- Smooth scroll for anchor links
- Staggered `fadeUp` animations via `IntersectionObserver`

## Deployment

The file is served statically (GitHub Pages or similar). The CNAME points to `blog.deepveloper.com`.
