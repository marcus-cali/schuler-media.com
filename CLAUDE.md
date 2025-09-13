# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

# Project: schuler-media.com

## Site Information

**URL**: https://schuler.media  
**Generator**: Hugo v0.147.0
**Theme**: minimal-llm (custom theme)
**Deployment**: Netlify (auto-deploy on push to GitHub)

## Commands

### Development
```bash
# Run local development server with drafts
hugo server -D

# Build site (outputs to /public/)
hugo

# Production build (used by Netlify)
hugo --gc --minify
```

## Architecture

This is a Hugo static site with a custom minimal-llm theme focused on professional media services presentation.

### Key Directories
- `/content/` - Markdown content files (homepage, about, contact, posts)
- `/themes/minimal-llm/` - Custom theme with responsive design
  - `/layouts/` - HTML templates for different content types
  - `/assets/css/` - Component-based CSS with CSS variables
- `/assets/css/home.css` - Custom homepage styling
- `/public/` - Generated static site (gitignored, never edit directly)

### Theme Architecture
- **Mobile-first responsive design** with hamburger menu for mobile
- **Component-based CSS** using modern CSS features (grid, flexbox, CSS variables)
- **SEO optimized** with structured data, meta tags, and sitemap generation
- **Performance focused** with minified builds and optimized assets

### Content Structure
- Homepage: Hero section, newsletter showcase (Implicator.ai, Filtr.de), services grid, recent work
- About/Contact pages: Standard content pages
- Blog posts: Located in `/content/posts/`

## Important Configuration

### hugo.toml
- Base URL: https://schuler.media/
- Outputs: HTML, RSS, JSON
- Goldmark renderer with unsafe HTML enabled (for custom HTML in markdown)

### netlify.toml
- Hugo version: 0.147.0
- Auto-builds on push with `hugo --gc --minify`
- Custom headers for SEO and content types

## Deployment Workflow
1. Make changes to content or theme
2. Test locally with `hugo server -D`
3. Commit and push to GitHub
4. Netlify automatically builds and deploys

## Recent Changes

### Blind Text Removal (December 2024)
- Removed test posts (post-1, post-2, post-3) containing Lorem ipsum content
- Site now displays only legitimate content

## Design Updates

- Preliminary design update initiated for project tracking and visual refinement

## Deployment Updates

- Dewsign update performed to enhance site deployment configuration
- 
## Standard Workflow

1. First think through the problem, read the codebase for relevant files, and write a plan to projectplan.md
2. The plan should have a list of todo items that you can check off as you complete them
3. Before you begin working, check in with me and I will verify the plan
4. Then, begin working on the todo items, marking them as complete as you go
5. Please every step of the way just give me a high level explanation of what changes you made
6. Make every task and code change you do as simple as possible. We want to avoid making any massive or complex changes. Every change should impact as little code as possible. Everything is about simplicity
7. Finally, add a review section to the projectplan.md file with a summary of the changes you made and any other relevant information
