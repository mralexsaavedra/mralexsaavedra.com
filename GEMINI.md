# GEMINI.md

This file provides guidance to Gemini CLI when working with code in this repository.

## Commands

```bash
pnpm dev          # Start dev server
pnpm build        # Type-check + production build
pnpm preview      # Preview production build
pnpm lint         # ESLint with auto-fix
pnpm format       # Prettier format
```

Package manager: **pnpm**. Node >= 24 (see `.nvmrc`).

## Stack

- **Astro 5** — static site, file-based routing (`src/pages/`)
- **Tailwind CSS 3** — semantic color system via CSS variables
- **TypeScript** — strict mode (`tsconfig.json` extends `astro/strict`)
- **IBM Plex** — Sans (body) + Mono (accents), WOFF2, preloaded

## Architecture

Single-page personal portfolio. Two routes: `/` and `/404`.

```
src/
  pages/       # index.astro (home), 404.astro
  layouts/     # Layout.astro — wraps every page (container, meta, fonts)
  components/  # SeoHead, ProjectItem, ExternalLink
  assets/      # global.css — Tailwind imports + CSS custom properties
public/        # fonts/, cv.pdf, banner.png, favicons
```

## Styling Conventions

Colors are **semantic CSS variables** (HSL), never raw values:

- `--background`, `--foreground`, `--primary`, `--muted`, `--accent`, `--border`, `--card`
- Tailwind extends these as named colors — use `text-foreground`, `bg-card`, etc.

Dark mode only (`darkMode: 'class'` + `dark` class on `<html>`).

## Component Conventions

All components define a `readonly` Props interface. Use `class:list` for dynamic classes, Astro slots for flexible content.

SEO meta (OG, Twitter, JSON-LD Schema.org) lives in `SeoHead.astro`.

## Git Hooks

Husky + lint-staged run on commit: ESLint auto-fix → Prettier format on staged `.ts` / `.astro` files. Do not skip hooks.
