# Chrome Extension Template Knowledge

## Project Overview

A minimal Chrome extension starter template with TypeScript, React, and Vite for modern extension development. Uses Manifest V3.

## Technology Stack

- **React 18** — UI for popup and options pages
- **TypeScript** — Type safety
- **Vite 5** — Fast build tool
- **ESLint** — Code linting with React hooks rules
- **Manifest V3** — Modern Chrome extension API

## Project Structure

```
src/
├── background/    # Service worker (Manifest V3)
├── content/       # Content scripts
├── popup/         # Extension popup UI (React)
└── options/       # Options page (React)

public/
└── manifest.json  # Extension manifest

dist/              # Built extension (load into Chrome)
```

## Key Commands

| Command | Description |
|---------|-------------|
| `npm run dev` | Build in watch mode for development |
| `npm run build` | Build for production |
| `npm run typecheck` | Run TypeScript type checking |
| `npm run lint` | Run ESLint with React hooks support |

## Verifying Changes

After every change, run:

```bash
npm run typecheck && npm run lint
```

This will check for:
- TypeScript type errors (strict mode)
- ESLint issues (React hooks rules, best practices)

## Extension Types

### Background Service Worker
Located in `src/background/`. Handles:
- Browser events (tabs, bookmarks, etc.)
- Long-running tasks
- Message passing between components

**Note:** Service worker cannot use DOM APIs.

### Content Scripts
Located in `src/content/`. Injected into:
- Specific pages based on `matches` in manifest
- Can modify DOM and communicate with background

**Note:** Content scripts have limited access to Chrome APIs.

### Popup UI
Located in `src/popup/`. A React app that:
- Opens when clicking the extension icon
- Has access to some Chrome APIs
- Limited lifetime (closes when user clicks away)

### Options Page
Located in `src/options/`. A React app for:
- User preferences and settings
- Persistent configuration

## Best Practices

- Keep service worker (background script) lightweight
- Use content scripts sparingly and only on needed pages
- Prefer using `storage.sync` over `storage.local` for user settings
- Follow Chrome's security best practices for CSP

## Development Workflow

- Always test extension in incognito mode to verify permissions
- Test on both HTTP and HTTPS sites if using content scripts
- Keep permissions minimal — request only what you need

## Chrome Web Store Publishing

Chrome Web Store requires:
- One-time $5 USD developer fee
- Detailed description and screenshots
- Privacy policy if collecting data
- Review process takes 1-3 business days