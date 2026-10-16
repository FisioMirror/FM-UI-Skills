---
name: morphicons
description: Use when icons should morph/animate from one shape into another (menu-to-X, play-to-pause, sun-to-moon) in React, Vue, Svelte, React Native or Astro. Triggers on "morph icons", "animate icon", "icon transition", "lucide morph", "hamburger to close".
---

# morphicons

`morphicons` (https://morphicons.com) morphs any stroke-based icon into any other with spring physics. Zero runtime deps, ~6.5 KB gzip. Rotations are solved mathematically (2D Procrustes + polar interpolation) — no hand-declared rotation groups.

- Repo: https://github.com/guillermolg00/morphicons
- Works with Lucide, Tabler, Heroicons outline, Iconoir, or raw SVG path data.
- Entry points: `morphicons/react`, `morphicons/vue`, `morphicons/svelte`, `morphicons/react-native`, `morphicons/astro`, `morphicons/element`.

## Install
```bash
npm install morphicons   # or: bun add morphicons / pnpm add morphicons
```
Icons come as DATA, not components. Import icon data from the icon package:
```tsx
import { MorphIcon } from "morphicons/react";
import { Menu, X } from "lucide";

<MorphIcon icon={open ? X : Menu} spring="snappy" />
```

## Modes
- Uncontrolled (90% of cases): change the `icon` prop and it morphs.
- Controlled: `<MorphIcon from={Menu} to={X} progress={dragProgress} />` (no spring).
- Imperative: ref with `morphTo(Icon)` / `set(Icon)`.

Props: `spring` ("smooth" | "snappy" | "bouncy"), `stroke`, `reducedMotion="user"` (defaults to always animate).

## When to use
- Toggle buttons, theme switches, play/pause, expand/collapse chevrons, tab icons.
- Keep it purposeful: morph only state-changing icons, not decorative ones (see `emil-design-eng`).

## Note
Peers are optional and version-gated: react >=18, vue >=3.3, svelte >=5, react-native >=0.71 + react-native-svg >=14. Confirm before adding.
