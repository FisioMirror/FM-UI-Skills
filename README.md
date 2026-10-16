# FM UI Skills

A curated, battle-tested library of **49 UI/UX, motion and anti-"AI-slop" agent skills**, packaged for [opencode](https://opencode.ai), Claude Code, Cursor and any tool that reads `SKILL.md` folders.

Built for **FisioMirror** to raise AI-generated interfaces to a deliberate, high-craft level — modern and highly animated, but professional and serious. **Enhance, never erase.**

## What's inside

```
skills/
  <skill-name>/
    SKILL.md          # frontmatter: name + description, plus instructions
    ...               # optional references, scripts, assets
```

## Install

These skills follow the common `SKILL.md` convention (YAML frontmatter with `name` and `description`).

- **opencode (global):** copy folders into `~/.config/opencode/skills/`
  ```bash
  git clone https://github.com/FisioMirror/FM-UI-Skills.git
  mkdir -p ~/.config/opencode/skills
  cp -r FM-UI-Skills/skills/* ~/.config/opencode/skills/
  ```
  Restart opencode — skills are loaded at startup.
- **opencode (per project):** copy into `<project>/.opencode/skills/`.
- **Claude Code:** copy into `~/.claude/skills/`.
- **Other tools:** point them at the `skills/` directory (each subfolder is one skill).

## Index

### Motion & animation (Emil Kowalski)
| Skill | What it does |
| --- | --- |
| `emil-design-eng` | Main skill: UI polish and when/how to animate. |
| `animate` | Build an animation — curve, duration, properties. |
| `animate-expo` | React Native / Expo motion (gestures, haptics, sheets). |
| `review-animations` | Strict review of animation code. |
| `improve-animations` | Audit + prioritized fix plan. |
| `find-animation-opportunities` | Where motion helps (and where it hurts). |
| `animation-performance` | Fix dropped frames. |
| `animation-vocabulary` | Precise words to ask an AI for motion. |
| `apple-design` | Apple's interface/motion principles for the web. |
| `mobile-native` | Make a web app feel native on phones. |
| `pick-ui-library` | Choose the right library instead of hand-rolling. |
| `prototype` | Build multiple UI variants with a switcher. |
| `break-ui` | Worst-case data stress test. |
| `ask-sonner` | Sonner toasts. |

### Visual direction & anti-slop
| Skill | What it does |
| --- | --- |
| `frontend-design` | Intentional visual direction (palette, type, layout). |
| `design-taste-frontend` | Infer a direction before writing code. |
| `high-end-visual-design` | Fix type/spacing/easing, ban AI defaults. |
| `brandkit` / `brand-guidelines` / `theme-factory` | Brand systems and theming. |
| `gpt-taste` / `stitch-design-taste` / `image-to-code` | Editorial / imagery-driven UI. |
| `industrial-brutalist-ui` / `minimalist-ui` | Specific aesthetic directions. |

### Review, improve & refine
| Skill | What it does |
| --- | --- |
| `ai-ui-refine` | Polish AI-generated UI without losing the good parts. |
| `impeccable` | 24 commands + 61 checks for AI-made interfaces. |
| `redesign-existing-projects` | Structure-preserving redesign. |
| `web-design-guidelines` | Vercel Web Interface Guidelines (file:line). |
| `accessibility-engineer` / `usability-psychologist` / `ui-designer` | UX and a11y. |
| `frontend-implementation` / `creative-coder` | Implementation craft. |
| `web-artifacts-builder` / `superdesign` / `canvas-design` | Artifact and canvas design. |

### React / framework craft
| Skill | What it does |
| --- | --- |
| `vercel-react-best-practices` | React best practices. |
| `vercel-composition-patterns` | Component composition patterns. |
| `vercel-react-view-transitions` | View Transitions API in React. |
| `vercel-react-native-skills` | React Native patterns. |
| `writing-guidelines` | Copy and microcopy. |

### Component libraries & effects
| Skill | What it does |
| --- | --- |
| `react-bits` | Animated copy-paste React components (reactbits.dev). |
| `morphicons` | SVG icon morphing. |
| `threejs-ui` | Three.js / React Three Fiber 3D components (threeui.com). |
| `loading-dev` | Beautiful React loading indicators. |
| `motion-design-tools` | Spline, Unicorn, Lottie, ProtoPie, inspiration sources. |

### Meta
| Skill | What it does |
| --- | --- |
| `ui-skills-index` | Master index — pick the right skill for a task. |

## Credits

Curated from public collections including Emil Kowalski's `skills`, Anthropic's `skills`, Leonxlnx `taste-skill`, `mae616/design-skills`, `pbakaus/impeccable`, `superdesigndev/superdesign-skill`, and `vercel-labs/agent-skills`, plus custom skills for the FisioMirror workflow. Respect each skill's original license where present.

## License

Repository structure and the `ai-ui-refine`, `react-bits`, `morphicons`, `loading-dev`, `threejs-ui`, `motion-design-tools` and `ui-skills-index` skills are MIT. Bundled third-party skills retain their original licenses.
