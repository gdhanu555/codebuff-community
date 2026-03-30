# Fishies — Animated Aquarium Knowledge

## Project Overview

An interactive underwater aquarium simulation with swimming fish, predators, and interactive elements. Built with React + Vite.

## Technology Stack

- **React 18** — UI library
- **TypeScript** — Type safety
- **Vite 5** — Build tool with fast HMR
- **CSS Animations** — Smooth creature movement

## Project Structure

```
src/
├── components/
│   ├── Fish.tsx         # Fish behavior and rendering
│   ├── Shark.tsx        # Predator AI
│   ├── WhaleShark.tsx   # Protective predator
│   ├── Starfish.tsx     # Bottom dweller
│   ├── Crab.tsx         # Territorial creature
│   ├── Jellyfish.tsx    # Drifting creature
│   ├── Coral.tsx        # Shelter decoration
│   ├── Seaweed.tsx      # Swaying decoration
│   ├── Bubble.tsx       # Interactive bubbles
│   ├── FoodPellet.tsx   # Interactive food
│   └── RippleEffect.tsx # Water ripples
├── App.tsx              # Main app component
├── App.css              # App styles
├── index.css            # Global styles
├── types.ts             # TypeScript types
└── main.tsx             # Entry point
```

## Key Commands

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run lint` | Run ESLint |
| `npm run typecheck` | TypeScript type check |
| `npm run preview` | Preview production build |

## Interactive Features

| Action | Effect |
|--------|--------|
| **Click** | Creates bubbles that float up |
| **Shift + Click** | Drops food pellets that fish eat |
| **Ctrl/Cmd + Click** | Creates sparkle effects |

## Marine Life

### Fish
- **Fish** — School together, flee from predators, seek food
- **Starfish** — Rest on the ocean floor
- **Crab** — Patrols the bottom territory
- **Jellyfish** — Drift lazily with the current

### Predators
- **Shark** — Hunts fish that get too close
- **Whale Shark** — Protects nearby fish from sharks

### Environment
- **Coral** — Provides shelter for fish
- **Seaweed** — Sways in the current
- **Seashells** — Decorative ocean floor items

## Behavior System

### Fish AI
- School with nearby fish for safety
- Flee when predators approach
- Seek food when hungry
- Hide near decorations when threatened
- Speed increases near predators

### Predator AI
- Sharks chase the nearest prey
- Whale sharks create a protection radius
- Predators compete for prey
- Ripple effects appear under fast movement

### Ecosystem Balance
- Base fish speed: 0.5 units
- Shark speed: 3 units
- Whale shark speed: 4 units
- Protection radius: 100px from whale shark

## Animation Guidelines

- Use CSS transitions for smooth movement
- Use 3D transforms for depth
- Scale with depth for dramatic effect
- Use rotateY for direction changes
- Remove transitions for immediate reactions (predator attacks)

## Verifying Changes

After every change, run:

```bash
npm run lint && npm run typecheck
```

This will check for:
- ESLint issues
- TypeScript type errors

## Extending the Aquarium

Ideas for extending with Codebuff:
- New creatures (octopus, seahorse, turtle)
- Sound effects and music
- Score tracking for feeding
- Different aquarium backgrounds
- Save/load aquarium state