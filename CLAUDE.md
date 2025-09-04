# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an Astro project using the "basics" starter template. It's a minimal static site generator setup with TypeScript support.

## Development Commands

All commands should be run from the project root:

| Command | Purpose |
|---------|---------|
| `npm run dev` | Start development server at `localhost:4321` |
| `npm run build` | Build production site to `./dist/` |
| `npm run preview` | Preview production build locally |
| `npm run astro ...` | Run Astro CLI commands (e.g., `npm run astro add`, `npm run astro check`) |

## Project Structure

```
src/
├── assets/          # Static assets (images, SVGs)
├── components/      # Reusable Astro components (.astro files)
├── layouts/         # Layout templates for pages
└── pages/           # Route-based pages (file-based routing)
```

## Architecture Notes

- **File-based routing**: Pages in `src/pages/` automatically become routes
- **Component architecture**: Uses `.astro` component format with frontmatter script sections
- **Styling**: Component-scoped CSS using `<style>` tags within `.astro` files
- **TypeScript**: Configured with strict TypeScript settings (`extends: "astro/tsconfigs/strict"`)
- **Layout system**: Base layout in `src/layouts/Layout.astro` provides HTML structure

## Key Files

- `src/pages/index.astro` - Homepage entry point
- `src/layouts/Layout.astro` - Main HTML layout template
- `src/components/Welcome.astro` - Main landing page component
- `astro.config.mjs` - Minimal Astro configuration
- `tsconfig.json` - TypeScript configuration with strict settings