# 🐠 Fishies — Animated Aquarium

An interactive underwater aquarium simulation with swimming fish, predators, and interactive elements. Built with React + Vite.

![Fishies Aquarium](https://github.com/user-attachments/assets/e1a5e6f5-a38a-42c2-955c-fa6de86750ec)

## Get This Project

```bash
codebuff --create fishies my-aquarium
```

## Getting Started

```bash
# Install dependencies
npm install

# Start the aquarium
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) to see your fish tank!

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

## Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run lint` | Run ESLint |
| `npm run typecheck` | TypeScript type check |
| `npm run preview` | Preview production build |

## Learn More

- [Vite Documentation](https://vitejs.dev/)
- [React Documentation](https://react.dev/)
- [Codebuff Docs](https://www.codebuff.com/docs)

## Extend the Aquarium

This is a great project to extend with Codebuff! Try adding:
- New creatures (octopus, seahorse, turtle)
- Sound effects and music
- Score tracking for feeding
- Different aquarium backgrounds
- Save/load aquarium state

---

Built with 💙 using [Codebuff](https://codebuff.com)