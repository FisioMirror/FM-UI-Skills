---
name: threejs-ui
description: Use when adding 3D effects to a web UI (hero scenes, interactive objects, shader backgrounds, Awwwards-level visuals) with Three.js / React Three Fiber. Triggers on "3D", "three.js", "threejs", "webgl", "shader", "3D hero", "threeui".
---

# Three.js UI (threeui.com)

`threeui` (https://threeui.com) is a collection of high-quality 3D Three.js components, templates, and prompts you can customize and drop into projects to reach "Awwwards-level" interfaces without starting from scratch.

## When to use
- A hero needs an interactive 3D object, floating geometry, or a shader background.
- You want a starting template rather than raw WebGL.
- You need prompts that generate Three.js scenes reliably.

## Workflow
1. Browse threeui.com for a component/template close to the goal.
2. Copy the Three.js / React Three Fiber code and adapt scene, materials, and camera.
3. In React, prefer `@react-three/fiber` + `@react-three/drei` for declarative scenes.
4. Lazy-load the canvas; keep it out of the critical path.

## Performance & craft (non-negotiable)
- Cap `dpr` (e.g. `[1, 2]`), pause the render loop when off-screen/hidden, and kill the RAF on unmount.
- Provide a static poster/fallback for reduced-motion and low-power devices.
- One hero 3D moment per page; don't share the GPU with a dozen animated widgets.
- Watch bundle size — Three.js is heavy; dynamic-import it.

## Related tools
- spline.design — no-code 3D, exportable to web.
- unicorn.studio — WebGL shaders/effects without writing GLSL.
- See the `motion-design-tools` skill for the full toolset.
