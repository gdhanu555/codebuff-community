# Codebuff Community Repository

This is the community repository for [Codebuff](https://codebuff.com), a CLI tool for AI-assisted coding. It contains starter templates and showcase projects built by the community.

## Quickstart

- **Install Codebuff**: `npm install -g codebuff`
- **Create a project**: `codebuff --create <template-name> my-project`
- **Start in existing directory**: `cd my-project && codebuff`

## Architecture

### Key Directories
- `/starter-templates` — Pre-configured project templates for various tech stacks
- `/showcase` — Community-built example projects
- `/utils` — Docker utilities for running Codebuff
- `/knowledge` — Knowledge files for specific topics

### Available Templates (in `/starter-templates`)
| Template | Description |
|----------|-------------|
| `nextjs` | Next.js 15 with React 19, TypeScript, Tailwind |
| `vite` | Vite + React 18, TypeScript, ESLint |
| `node-cli` | Node.js CLI with TypeScript, tsx for dev |
| `python-cli` | Python CLI with Hatch, Black, MyPy |
| `remix` | Remix with Vite, TypeScript, Tailwind |
| `chrome-extension` | Chrome Extension with Vite, React |
| `convex` | Convex full-stack template |

### Showcase Projects (in `/showcase`)
- `fishies` — Animated underwater aquarium (React + Vite)
- `minecraft-complex` — Minecraft-inspired 3D UI (Remix + Tailwind)
- `minecraft-simple` — Simple Minecraft demo (vanilla JS)
- `code-analysis` — Git analysis CLI + Chrome extension (Python)

## Commands

Commands vary by project. Common patterns:

### Node.js Projects (Next.js, Vite, Remix, etc.)
```bash
npm install        # Install dependencies
npm run dev        # Start dev server
npm run build      # Build for production
npm run lint       # Run ESLint
npm run typecheck  # Run TypeScript compiler
```

### Python Projects
```bash
pip install -e ".[dev]"  # Install with dev dependencies
python -m cli            # Run CLI
pytest                   # Run tests
black .                  # Format code
mypy .                   # Type check
```

### Template-specific
- **node-cli**: `npm run dev` (uses tsx), `npm run build` (compiles to dist/)
- **python-cli**: Uses Hatch for packaging, `hatch run` for commands

## Conventions

- Each template has its own `package.json` / `pyproject.toml` — manage dependencies per-project
- All templates include a `codebuff.json` configuration file
- TypeScript projects use strict mode
- Python projects use Black formatting (88-char line length) and strict MyPy
- Each project has its own knowledge.md with specific guidance

## Gotchas

- This is a **meta-repository** — individual projects manage their own dependencies
- When adding a new template, include `package.json`, `tsconfig.json`, and a starter `knowledge.md`
- Showcase projects can be git submodules (see `.gitmodules`)
- Python CLI uses Hatchling as the build backend
- Node.js CLI templates use `tsx` for development (not ts-node)