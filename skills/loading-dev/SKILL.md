---
name: loading-dev
description: Use when you need beautiful, customizable loading spinners/indicators for React (buttons, suspense fallbacks, data fetches). Triggers on "loading spinner", "loading indicator", "loading animation", "skeleton spinner", "loading.dev".
---

# loading.dev

`loading-dev` (https://loading.dev) is a lightweight library of beautiful React loading indicators. Repo: https://github.com/jakubkrehel/loading

## Install
```bash
npm install loading-dev
```

## Usage
```tsx
import { Arc, Atom, Blocks, Comet, Ripple } from "loading-dev";
<Arc size={16} />
```
Every indicator supports `size`, `color`, `duration`; some expose `easing`, `cap`, and spinner-specific props. The library exposes `playState` and lets you override styles. Spinners respect reduced motion automatically.

## Catalog (pick by vibe)
- Minimal/clean: Arc, Ring, Comet, Orbit, Dual, Classic, ClassicV2
- Dots: BouncingDots, CircularDots, LinearDots, Leap, Eclipse
- Geometric: Blocks, Flip, Gather, Swirl, Snake, Trace
- Organic: Pulse, Ripple, Wave, Cascade, Atom, Morph
- Brand: Loading, Clock, Slide

## Rules
- Match the indicator's weight to the UI (16px inside buttons, larger for page-level).
- Prefer one consistent loader across the app.
- Respect reduced motion (already handled) and avoid flashing for <300ms operations.

## Note
Requires React 19+. The user's project is on React 18 — if used, either upgrade React (careful: HeroUI 3 wants React 19) or fall back to a lighter spinner (e.g. a CSS spinner). Confirm before installing.
