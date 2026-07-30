# Attune

A static marketing site for **Attune** — a fictional enterprise coaching platform built as a UX case study.
Nothing here is a real product; all content, naming, and metrics are original and illustrative.

> The coaching platform that develops every person — and proves every gain.

## Pages

| File | What it is |
|---|---|
| `index.html` | Entry point — redirects to the home page |
| `Attune Hero.dc.html` | Home page |
| `Attune Platform.dc.html` | Platform overview |
| `Attune Guide.dc.html` | Attune Guide (1:1 human coaching) product page |
| `Attune Solutions.dc.html` | Solutions |
| `Attune Customers.dc.html` | Customers / case studies |
| `AttuneNav.dc.html` | Mega-menu nav component (standalone preview) |
| `AttuneFooter.dc.html` | Footer component (standalone preview) |

## How it's built

The pages were authored in Claude Design and exported as `.dc.html` files. Each one is a
self-contained document: markup, styles, and a small component class live in the same file.
`support.js` is the shared `dc-runtime` that mounts them (it pulls React from unpkg at runtime,
so the pages need network access to render). It is generated — don't hand-edit it.

Fonts come from Google Fonts (Fraunces for display, Inter for text), and the photography and
video are hot-linked from Unsplash and Pexels. Everything is loaded from a CDN — there are no
build steps, no dependencies to install, and no local image assets.

The filenames are kept exactly as exported so pages can be re-exported from Claude Design and
dropped back in without rewriting the cross-page links.

## Running locally

Serve the directory over HTTP — opening the files directly from disk won't work reliably:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploying

`.github/workflows/pages.yml` publishes the repo root to GitHub Pages on every push to `main`
(and to the current working branch), and can be run manually from the Actions tab.

One-time setup: **Settings → Pages → Build and deployment → Source: GitHub Actions**.

`.nojekyll` is present so Pages serves the files verbatim instead of running them through Jekyll.

## Design source material

`design/` holds the reference material the site was built from:

- `attune-brand-brief.md` — brand system, palette, voice, page content
- `attune-nav-and-pages-prompts.md` — the nav map and per-page build prompts
- `attune-hero.html` — an earlier standalone version of the hero
- screenshots and reference images
