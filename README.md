# Layout & Stack Advisor

> Educational application for beginners to visually select layouts and tech stacks with smart hints from a mentor.

## Features

- **47 CSS Grid Layouts** organized in 7 categories
- **Visual Constructor** with live preview
- **Smart Mentor Tips** with conflict detection
- **Theme Customization** (light/dark, fonts, colors)
- **Fullscreen Preview Mode**
- **localStorage Persistence**

## Categories

| Category | Count | Description |
|----------|-------|-------------|
| Basic | 5 | Simple universal layouts |
| Grid Classic | 5 | Time-tested patterns |
| Bento | 4 | Japanese style grid |
| Fibonacci | 13 | Nature proportions (1, 1, 2, 3, 5, 8...) |
| Math | 11 | Golden ratio, Pi, primes, roots |
| Advanced | 7 | Creative solutions |
| Complex | 2 | Dashboard, Blog |

## Tech Stack

- **Framework:** Next.js 16 (App Router, Turbopack)
- **Language:** TypeScript 5
- **Styling:** Tailwind CSS 4 + shadcn/ui (New York style)
- **State:** Zustand with localStorage persistence
- **Icons:** Lucide React

## Getting Started

```bash
# Clone the repository
git clone https://github.com/username/layout-advisor.git

# Install dependencies
cd layout-advisor
bun install

# Copy environment variables
cp .env.example .env

# Start development server
bun run dev
```

## Scripts

```bash
bun run dev      # Start development server
bun run build    # Build for production
bun run lint     # Run ESLint
bun run start    # Start production server
```

## Project Structure

```
src/
+-- types/layout.ts         # TypeScript interfaces
+-- data/layouts.ts         # Layout definitions (47 layouts)
+-- store/useAppStore.ts    # Zustand store
+-- components/
|   +-- layout-advisor/     # Main components
|   +-- ui/                 # shadcn/ui components
+-- app/
    +-- page.tsx            # Main page
    +-- globals.css         # Global styles
```

## Standards

This project follows:
- No-Unicode Policy v2.0
- Z.ai Reproducibility Standard v1.0
- Worklog System v2.0

## License

MIT

---

Built with: Next.js 16 + TypeScript + Tailwind CSS
