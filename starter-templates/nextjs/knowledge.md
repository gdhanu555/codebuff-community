# Next.js Template Knowledge

## Project Overview

A Next.js 15 project with React 19, TypeScript, and Tailwind CSS. Uses Turbopack for lightning-fast development and the App Router for modern routing.

## Technology Stack

- **Next.js 15** — React framework with App Router
- **React 19** — UI library
- **TypeScript** — Type safety
- **Tailwind CSS** — Utility-first CSS
- **Turbopack** — Next.js 15's Rust-based bundler

## Project Structure

```
app/
├── globals.css     # Global Tailwind styles
├── layout.tsx      # Root layout (includes Geist font)
└── page.tsx        # Home page

public/             # Static assets
next.config.ts      # Next.js configuration
tailwind.config.ts  # Tailwind CSS config
postcss.config.mjs  # PostCSS config
tsconfig.json       # TypeScript config
```

## Key Commands

| Command | Description |
|---------|-------------|
| `npm run dev` | Start dev server with Turbopack |
| `npm run build` | Build for production |
| `npm run start` | Start production server |
| `npm run lint` | Run ESLint |
| `npm run checks` | Run TypeScript + ESLint |

## Verifying Changes

After every change, run:

```bash
npm run checks
```

This runs `tsc --noEmit` (TypeScript) and `npm run lint` (ESLint).

## Code Quality Standards

- TypeScript strict mode
- Next.js ESLint configuration
- Tailwind CSS best practices
- ESLint with React hooks rules

## App Router Conventions

- `app/layout.tsx` — Root layout, wraps all pages
- `app/page.tsx` — Home page (default route)
- `app/globals.css` — Global styles and Tailwind imports
- Static assets go in `public/`