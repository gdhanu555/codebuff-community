# Vite + React Template Knowledge

## Project Overview

A minimal React + TypeScript starter template using Vite for fast development and building. Perfect for single-page applications, prototypes, and learning React.

## Technology Stack

- **React 18** — UI library
- **TypeScript** — Type safety
- **Vite 6** — Build tool with fast HMR
- **ESLint 9** — Code linting
- **ESLint React Hooks** — Hooks rules enforcement

## Project Structure

```
src/
├── main.tsx      # Entry point
├── App.tsx       # Root component
├── App.css       # App styles
└── index.css     # Global styles

index.html        # HTML template
vite.config.ts    # Vite configuration
tsconfig.json     # TypeScript configuration
eslint.config.js  # ESLint configuration
```

## Verifying Changes

After every change, run:

```bash
npm run lint && npm run typecheck
```

This will check for:
- ESLint issues (React hooks rules, best practices)
- TypeScript type errors (strict mode)

## Key Commands

| Command | Description |
|---------|-------------|
| `npm run dev` | Start dev server with HMR |
| `npm run build` | Production build |
| `npm run preview` | Preview production build |
| `npm run lint` | Run ESLint |
| `npm run typecheck` | TypeScript type check |