# CLAUDE.md

## Project Overview

Personal website for Jim Zenn (jimzenn.com), built with Hugo. The site contains a personal timeline, blog posts, academic math notes (with LaTeX), and a resume.

## Branch Structure

- **`hugo`** — Source branch. All development happens here.
- **`master`** — Built site (GitHub Pages deployment target). Do not edit directly.

## Build & Dev

```bash
hugo              # Build site to public/
hugo server       # Dev server at localhost:1313
```

Requires Hugo extended v0.151.0+. Install via `brew install hugo`.

## Project Structure

```
hugo.toml            # Site config (title, params, taxonomies)
content/             # Markdown content
  _index.md          # Home page
  about.md, resume.md, journey.md, blog.md  # Top-level pages
  analysis/          # Math notes (layout: note)
  linear-algebra/
  optimization/
  probability-theory/
  dynamics/
  blog/              # Blog posts
data/                # YAML data files
  menu.yaml          # Navigation menu
  subjects.yaml      # Academic course metadata
  featured_photos.yaml  # Jumbotron photo gallery
  resume/general.yaml   # Resume structured data
static/              # Static assets (copied as-is to public/)
  css/               # All CSS files (16 files)
  images/            # Featured photos (jpg, webp, original)
  fonts/             # (empty — fonts loaded from Google Fonts CDN)
  favicon.png, favicon-dark.png, favicon-light.png
layouts/             # Local template overrides (take precedence over theme)
  _default/          # baseof, note, resume, subject
  partials/          # head, jumbotron, pagination, scripts
  shortcodes/        # Only site-specific overrides (solution.html)
  taxonomy/          # tag.terms
  rss.xml
themes/zealoft/      # Theme submodule (git@github.com:Jim-Zenn/hugo-theme-zealoft.git)
```

## Architecture Decisions

### CSS: All in static/css/, using relURL
All CSS is served from `static/css/` via `relURL` with `?v=` cache-busting suffix. Both theme and site-level templates use the same pattern: `{{ "css/file.css" | relURL }}?v={{ .Site.Params.version }}`. Theme CSS lives in `themes/zealoft/static/css/`, site overrides in `static/css/`.

### Theme Overrides
The zealoft theme is a git submodule. Do not edit files inside `themes/zealoft/` — create local overrides in `layouts/` instead. Hugo's lookup order means project-level layouts take precedence.

### Font Stack
```css
--display-font: -apple-system, BlinkMacSystemFont, "Inter", sans-serif;
--text-font: -apple-system, BlinkMacSystemFont, "Inter", sans-serif;
```
Apple's SF Pro is used via system font keywords (no self-hosted files — Apple's license prohibits it). Inter is loaded from Google Fonts as fallback. Defined in `static/css/root.css`.

### Math Rendering
MathJax 3 via CDN (`tex-chtml` component). Configured in `layouts/partials/scripts.html`. Supports `$...$` inline and `$$...$$` display math. AMS equation numbering enabled.

### Taxonomies
Custom taxonomy names in hugo.toml:
- `category = "volumes"` (chapter/section grouping for notes)
- `tag = "keywords"` (content tags)

Use lowercase in `.Param` calls: `.Param "volumes"`, `.Param "issue"`.

## Content Conventions

### Math Notes
Frontmatter pattern:
```yaml
title: "Section Title"
date: 2018-08-06T11:03:48+08:00
volumes: ["1"]
layout: "note"
type: "notes"
issue: 3
weight: 103
```

### Blog Posts
```yaml
title: "Post Title"
date: 2019-11-13T12:11:48+08:00
volumes: ["Journey"]
```

### Shortcodes
11 block-type shortcodes (`theorem`, `definition`, `lemma`, `corollary`, `proposition`, `example`, `note`, `recall`, `remarks`, `properties`, `axioms`) are unified via `themes/zealoft/layouts/partials/shortcodes/block.html`. Each shortcode file is a one-line call passing color, title, and keyword config. Additionally: `proof` and `solution` (expandable/collapsible). All use `{{ .Site.Params.email }}` for contact links.

## Key Config Values

- `params.email` — Used by shortcode mailto links
- `params.version` — Appended to CSS URLs for cache busting
- `params.themeColor` — Sets `--backdrop-color` CSS variable and meta theme-color

## External Dependencies (CDN)

- jQuery 3.7.1 slim (code.jquery.com) — Loaded only on resume page, used for print function
- MathJax 3 (cdn.jsdelivr.net) — LaTeX rendering
- Google Fonts: Inter (weights 400, 500, 600, 700 only)
- p5.js (cdnjs.cloudflare.com) — Game of Life animation on home page
