# jimzenn.com

Personal website of Jim Zenn — [jimzenn.com](https://jimzenn.com/)

Built with [Hugo](https://gohugo.io/) using the custom [Zealoft](https://github.com/Jim-Zenn/hugo-theme-zealoft) theme.

## Setup

```bash
# Clone with submodule
git clone --recurse-submodules git@github.com:Jim-Zenn/jimzenn.github.io.git
cd jimzenn.github.io
git checkout hugo

# Install Hugo (macOS)
brew install hugo

# Dev server
hugo server
```

Requires Hugo extended v0.151.0+.

## Branches

| Branch | Purpose |
|--------|---------|
| `hugo` | Source code (develop here) |
| `master` | Built site (GitHub Pages) |

## Structure

```
config.toml       Site configuration
content/          Markdown content (pages, blog, math notes)
data/             YAML data (menu, resume, subjects, photos)
static/           CSS, images, PDFs, favicons
layouts/          Template overrides for the Zealoft theme
themes/zealoft/   Theme (git submodule)
```

## Content

- **Home** — Personal timeline with featured photo jumbotron
- **Blog** — Essays and reflections
- **Notes** — Math lecture notes with LaTeX (Analysis, Linear Algebra, Probability Theory, Optimization, Dynamics)
- **Resume** — Structured resume from YAML data

## Build

```bash
hugo                    # Build to public/
hugo server             # Dev server at localhost:1313
hugo server --buildDrafts  # Include draft content
```
