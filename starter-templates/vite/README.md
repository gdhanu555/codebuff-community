# Vite + React Template

A minimal React + TypeScript starter template using [Vite](https://vitejs.dev/) for fast development and building. Perfect for single-page applications, prototypes, and learning React.

## Get This Template

```bash
codebuff --create vite my-app
```

## Quick Start

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) to see your app.

## Available Commands

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server with HMR |
| `npm run build` | Build for production (TypeScript + Vite) |
| `npm run lint` | Run ESLint with React hooks support |
| `npm run typecheck` | Run TypeScript type checking |
| `npm run preview` | Preview production build locally |

## Project Structure

```
my-app/
├── src/
│   ├── main.tsx      # Entry point
│   ├── App.tsx       # Root component
│   ├── App.css       # App styles
│   └── index.css     # Global styles
├── index.html        # HTML template
├── package.json
├── tsconfig.json
├── vite.config.ts
└── eslint.config.js
```

## Technology Stack

- **React 18** — UI library
- **TypeScript** — Type safety
- **Vite 6** — Build tool with fast HMR
- **ESLint 9** — Code linting
- **ESLint React Hooks** — Hooks rules enforcement

## Code Quality

This template enforces:
- TypeScript strict mode
- React hooks best practices
- ES2022+ features

Run full checks:
```bash
npm run lint && npm run typecheck
```

## Learn More

- [Vite Documentation](https://vitejs.dev/)
- [React Documentation](https://react.dev/)
- [TypeScript Handbook](https://www.typescriptlang.org/docs/)
- [Codebuff Docs](https://www.codebuff.com/docs)
