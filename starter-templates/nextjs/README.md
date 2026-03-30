# Next.js Template

A [Next.js](https://nextjs.org) 15 project with React 19, TypeScript, and Tailwind CSS. Uses Turbopack for lightning-fast development.

## Get This Template

```bash
codebuff --create nextjs my-app
```

## Quick Start

```bash
# Install dependencies
npm install

# Start development server (uses Turbopack)
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to see your app.

Edit the page by modifying `app/page.tsx` — the page auto-updates as you save.

## Available Commands

| Command | Description |
|---------|-------------|
| `npm run dev` | Start dev server with Turbopack |
| `npm run build` | Build for production |
| `npm run start` | Start production server |
| `npm run lint` | Run ESLint |
| `npm run checks` | Run TypeScript + ESLint |

## Project Structure

```
my-app/
├── app/
│   ├── globals.css     # Global Tailwind styles
│   ├── layout.tsx      # Root layout
│   └── page.tsx        # Home page
├── public/             # Static assets
├── package.json
├── next.config.ts      # Next.js configuration
├── tailwind.config.ts  # Tailwind CSS config
├── postcss.config.mjs  # PostCSS config
└── tsconfig.json       # TypeScript config
```

## Technology Stack

- **Next.js 15** — React framework with App Router
- **React 19** — UI library
- **TypeScript** — Type safety
- **Tailwind CSS** — Utility-first CSS
- **Turbopack** — Next.js 15's Rust-based bundler

## Code Quality

This template enforces:
- TypeScript strict mode
- Next.js ESLint configuration
- Tailwind CSS best practices

Run all checks before committing:

```bash
npm run checks
```

This runs `tsc --noEmit` and `npm run lint`.

## Learn More

- [Next.js Documentation](https://nextjs.org/docs) — Features and API
- [Learn Next.js](https://nextjs.org/learn) — Interactive tutorial
- [Tailwind CSS](https://tailwindcss.com/docs)
- [Codebuff Docs](https://www.codebuff.com/docs)

## Deploy on Vercel

The easiest way to deploy is using the [Vercel Platform](https://vercel.com/new):

1. Push your code to GitHub
2. Import the project in Vercel
3. Deploy with zero configuration

See [Next.js deployment docs](https://nextjs.org/docs/app/building-your-application/deploying) for more options.