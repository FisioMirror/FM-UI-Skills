---
name: react-bits
description: Use when building eye-catching React UI with animated text, backgrounds, cards, cursors or micro-interactions. Triggers on "react-bits", "reactbits", "animated text", "animated background", "aurora", "spotlight card", "copy-paste React components", or when the user wants agency-level visual effects fast.
---

# React Bits

React Bits (https://reactbits.dev) is a free, open-source collection of 100+ animated, copy-paste React components: animated text, animated backgrounds, cards, click/cursor effects, and micro-interactions.

## When to use
- You need a striking hero, animated headline, aurora/particle background, spotlight card, marquee, or cursor trail.
- The user wants "wow" visuals without building effects from scratch.
- You want components that are customizable via props and droppable into an existing React + Tailwind project.

## How to use
1. Open https://reactbits.dev and pick a component. Each has a live playground where you tune parameters in real time.
2. Choose the JS/TS + Tailwind variant. Copy the code (the site gives the exact component file and required deps, often `motion` / `@react-spring/web`).
3. Drop the file into `src/components/` and import it. Most components accept props for speed, colors, size, and behavior.
4. Ask before installing new animation dependencies (e.g. `motion`, `gsap`, `three`) — check `package.json` first.

## Rules of craft (keep it classy)
- Effects are a highlight, not wallpaper. Use ONE hero effect, not five competing ones.
- Respect `prefers-reduced-motion`; provide a static fallback.
- Keep backgrounds subtle behind real content; watch contrast/legibility.
- Pair with the `emil-design-eng`, `review-animations`, and `high-end-visual-design` skills so motion feels intentional, not generic.

## Notes
- Works with React + Tailwind (the user's stack: React 18, Tailwind, framer-motion already present).
- Install hints use npm/bun; but never add a dependency without confirming.
