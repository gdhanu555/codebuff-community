# Node.js CLI Template

A minimal Node.js CLI application template with TypeScript support. Uses ES Modules and `tsx` for fast development.

## Get This Template

```bash
codebuff --create node-cli my-app
```

## Quick Start

```bash
# Install dependencies
npm install

# Run in development (uses tsx for hot reload)
npm run dev

# Build for production
npm run build

# Run the built CLI
npm start
```

## Available Commands

| Command | Description |
|---------|-------------|
| `npm run dev` | Run in development with tsx (hot reload) |
| `npm run build` | Compile TypeScript to JavaScript |
| `npm run start` | Run the compiled CLI from `dist/` |
| `npm run typecheck` | Run TypeScript type checking |

## Project Structure

```
my-app/
├── src/
│   └── index.ts       # Source code entry point
├── dist/              # Compiled JavaScript (git-ignored)
├── package.json
├── tsconfig.json
└── README.md
```

## Making the CLI Executable

After building, you can run the CLI directly:

```bash
# Make executable (optional)
chmod +x dist/index.js

# Run directly
./dist/index.js

# Or use node
node dist/index.js
```

## Technology Stack

- **Node.js** — Runtime (ES2022 target)
- **TypeScript** — Type safety
- **tsx** — Fast development execution (no compile step in dev)
- **ES Modules** — Native ESM (`"type": "module"`)

## Code Quality

This template enforces:
- TypeScript strict mode
- ES Modules best practices
- Modern Node.js features

Run type checking:
```bash
npm run typecheck
```

## Learn More

- [Node.js Documentation](https://nodejs.org/docs/)
- [TypeScript Handbook](https://www.typescriptlang.org/docs/)
- [tsx Documentation](https://github.com/privatenumber/tsx)
- [Codebuff Docs](https://www.codebuff.com/docs)