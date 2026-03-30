# Chrome Extension Template

A minimal Chrome extension starter template with TypeScript, React, and Vite for modern extension development. Uses Manifest V3.

## Get This Template

```bash
codebuff --create chrome-extension my-extension
```

## Quick Start

```bash
# Install dependencies
npm install

# Start development build with watch mode
npm run dev

# Build for production
npm run build
```

## Available Commands

| Command | Description |
|---------|-------------|
| `npm run dev` | Build in watch mode for development |
| `npm run build` | Build for production |
| `npm run typecheck` | Run TypeScript type checking |
| `npm run lint` | Run ESLint with React hooks support |

## Project Structure

```
my-extension/
├── src/
│   ├── background/    # Service worker (Manifest V3)
│   ├── content/       # Content scripts
│   ├── popup/         # Extension popup UI (React)
│   └── options/       # Options page (React)
├── public/
│   └── manifest.json  # Extension manifest
├── dist/              # Built extension (load into Chrome)
├── package.json
├── tsconfig.json
├── vite.config.ts
└── eslint.config.js
```

## Loading the Extension

1. Build the extension: `npm run build`
2. Open Chrome and navigate to `chrome://extensions`
3. Enable **Developer mode** (top-right toggle)
4. Click **Load unpacked** and select the `dist` directory
5. Pin the extension to your toolbar to test

## Technology Stack

- **React 18** — UI for popup and options pages
- **TypeScript** — Type safety
- **Vite 5** — Fast build tool
- **ESLint** — Code linting with React hooks rules
- **Manifest V3** — Modern Chrome extension API

## Code Quality

This template enforces:
- TypeScript strict mode
- React hooks best practices
- ESLint with React refresh

Run verification:
```bash
npm run typecheck && npm run lint
```

## Extension Types

### Background Service Worker
Located in `src/background/`. Handles:
- Browser events (tabs, bookmarks, etc.)
- Long-running tasks
- Message passing between components

### Content Scripts
Located in `src/content/`. Injected into:
- Specific pages based on `matches` in manifest
- Can modify DOM and communicate with background

### Popup UI
Located in `src/popup/`. A React app that:
- Opens when clicking the extension icon
- Has access to some Chrome APIs
- Limited lifetime (closes when user clicks away)

### Options Page
Located in `src/options/`. A React app for:
- User preferences and settings
- Persistent configuration

## Learn More

- [Chrome Extension Documentation](https://developer.chrome.com/docs/extensions)
- [Chrome Extension Samples](https://developer.chrome.com/docs/extensions/samples)
- [Manifest V3 Migration Guide](https://developer.chrome.com/docs/extensions/mv3/intro/)