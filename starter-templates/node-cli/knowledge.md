# Node CLI Template Knowledge

## Project Overview

A minimal Node.js CLI application template with TypeScript support. Uses ES Modules and `tsx` for fast development.

## Technology Stack

- **Node.js** — Runtime (ES2022 target)
- **TypeScript** — Type safety
- **tsx** — Fast development execution (hot reload, no compile in dev)
- **ES Modules** — Native ESM (`"type": "module"` in package.json)

## Project Structure

```
src/
└── index.ts       # Source code entry point

dist/              # Compiled JavaScript (git-ignored)
package.json       # CLI bin: "cli": "dist/index.js"
tsconfig.json      # TypeScript config
```

## Key Commands

| Command | Description |
|---------|-------------|
| `npm run dev` | Run in development with tsx (hot reload) |
| `npm run build` | Compile TypeScript to JavaScript |
| `npm run start` | Run the compiled CLI from `dist/` |
| `npm run typecheck` | Run TypeScript type checking |

## Verifying Changes

After every change, run:

```bash
npm run typecheck
```

This will check for TypeScript type errors (strict mode).

## Running the CLI

After building:

```bash
# Using npm start
npm start

# Or directly with node
node dist/index.js

# Or as executable (after chmod +x)
./dist/index.js
```

## Code Quality Standards

- TypeScript strict mode
- ES Modules best practices
- ES2022+ features