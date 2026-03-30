# Layout & Stack Advisor - Initial Prompt

> Project specification document. Source of truth for development.

---

## Project Overview

**Name:** Layout & Stack Advisor  
**Version:** 2.0  
**Purpose:** Educational application for beginners to visually select layouts and tech stacks with smart hints from a "mentor"

---

## Technical Requirements

### Core Stack
- **Framework:** Next.js 16 with App Router (Turbopack)
- **Language:** TypeScript 5
- **Styling:** Tailwind CSS 4 with shadcn/ui component library (New York style)
- **State Management:** Zustand with localStorage persistence
- **Icons:** Lucide React

### Component Architecture
- React functional components with hooks
- TypeScript strict mode
- shadcn/ui components (New York style, border-radius: 0.25rem)

---

## Functional Requirements

### 1. Goal Selector
- Project types: Landing, Admin Panel, Blog, E-commerce
- Displayed in header
- Affects recommendations and conflict detection

### 2. Visual Constructor
- Layout cards organized by categories
- Categories: Basic, Grid Classic, Bento, Fibonacci, Math, Advanced, Complex
- Visual preview for each layout
- CSS Grid code snippets

### 3. Live Preview
- Interactive layout visualization
- Fullscreen mode
- Real-time structure rendering

### 4. Theme Settings
- Light/Dark mode toggle
- Accent color presets
- Font family selection (sans, serif, mono)
- Font size options (S, M, L)

### 5. Smart Hints System
- Conflict detection between layout and project goal
- Best match recommendations
- Learning resources links
- Collapsible advisor panel in footer

### 6. Data Persistence
- localStorage for user preferences
- Zustand store with persist middleware

---

## Layout Categories (Total: 47 layouts)

| Category | Count | Description |
|----------|-------|-------------|
| Basic | 5 | Simple universal layouts |
| Grid Classic | 5 | Time-tested patterns |
| Bento | 4 | Japanese style grid |
| Fibonacci | 13 | Nature proportions (1, 1, 2, 3, 5, 8...) |
| Math | 11 | Golden ratio, Pi, primes, roots |
| Advanced | 7 | Creative solutions |
| Complex | 2 | Dashboard, Blog |

---

## UI/UX Requirements

- Responsive design (mobile-first)
- Sticky footer
- Dark theme support via CSS variables
- Accessible components (ARIA, semantic HTML)
- Loading states and error handling

---

## File Structure

```
src/
+-- types/layout.ts         # TypeScript interfaces
+-- data/layouts.ts         # Layout definitions
+-- store/useAppStore.ts    # Zustand store
+-- components/
|   +-- layout-advisor/
|   |   +-- GoalSelector.tsx
|   |   +-- LayoutSelector.tsx
|   |   +-- PreviewArea.tsx
|   |   +-- ThemeSettings.tsx
|   |   +-- AdvisorPanel.tsx
|   +-- ui/                 # shadcn/ui components
+-- app/
    +-- page.tsx            # Main page
    +-- layout.tsx
    +-- globals.css
```

---

## Standards Compliance

This project follows:
- No-Unicode Policy v2.0
- Z.ai Reproducibility Standard v1.0
- Worklog System v2.0

---

## Formula

```
clone + install + dev = working app
```

---

**Document Version:** 1.0  
**Created:** 2025-03-23
