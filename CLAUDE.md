# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal portfolio website for Michael Harp built with Jekyll and hosted on GitHub Pages at mikeharp.com.

## Development Commands

```bash
# Install dependencies
bundle install

# Run local development server (http://localhost:4000)
bundle exec jekyll serve

# Build static site to _site/
bundle exec jekyll build
```

## Architecture

- **Static Site Generator:** Jekyll 3.10 with GitHub Pages gem
- **Theme:** jekyll-theme-cayman with custom CSS overrides
- **Content:** Markdown files (index.md, contact.md) with YAML front matter

### Key Files

- `_config.yml` - Jekyll configuration (title, description, theme)
- `_layouts/default.html` - Main HTML template with data-driven navigation
- `_includes/head-custom.html` - Custom CSS (purple gradient, animations, modern styling)
- `_data/navigation.yml` - Navigation menu items
- `CNAME` - Custom domain configuration

### Content Flow

Pages are written in Markdown → processed by Jekyll using the default layout → navigation pulled from `_data/navigation.yml` → custom styles injected via `head-custom.html` → static HTML output to `_site/`.
