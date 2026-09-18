# 05 — Design resources

A curated source library for design inspiration, systems, tools, components and references that are especially useful when working with AI agents.

The goal is not to collect every beautiful website on the internet.

The goal is to collect sources that are:

- visually strong
- useful for extracting reusable principles
- structured enough for an AI agent to inspect and reason about
- concrete enough to support implementation
- broad enough to help us discover directions we would not invent from scratch

This file should stay curated. Add sources because they are useful, not because they exist.

---

# 1. How to use this library with AI

Not all reference sources are equally useful to an agent.

## Preferred source order

When possible, use this order:

1. **Inspect-able Figma file / design system**
2. **GitHub repository with source code + documentation**
3. **Official component / design-system documentation**
4. **A complete product flow or interaction recording**
5. **A well-curated gallery with direct project links**
6. **A screenshot or moodboard**

The closer a source is to actual structure, behaviour and code, the less the agent has to guess.

## AI readability scale

This document uses a rough scale:

- `★★★★★` — excellent for AI interpretation; structured docs/code/components
- `★★★★☆` — very useful; clear examples plus enough context
- `★★★☆☆` — visually useful but needs human explanation
- `★★☆☆☆` — mood / discovery only; use carefully

## Reference rule

Never say only:

> Make it like this.

Instead say:

```text
REFERENCE:
[url]

USE FOR:
- hierarchy
- interaction
- typography

BORROW:
- oversized primary control
- restrained colour
- visible state transitions

DO NOT BORROW:
- exact palette
- branding
- component arrangement
```

The source provides evidence. `design-dna` provides interpretation.

---

# 2. UI / UX inspiration

## Mobbin

https://mobbin.com/

**Best for:** real mobile and web products, complete flows, onboarding, checkout, navigation, account patterns.

**AI usefulness:** `★★★★☆`

Mobbin is most useful when we need to answer:

> How do mature products solve this interaction?

Use it for product behaviour and information architecture more than visual identity.

**Good prompts:**

- compare three real-world onboarding patterns
- study how apps expose secondary settings
- find examples of dense information without dashboard clutter

---

## Page Flows

https://pageflows.com/

**Best for:** UX flows, screen sequences, user journeys, interaction patterns.

**AI usefulness:** `★★★★☆`

Especially useful when the problem is **what happens next**, not simply how one screen looks.

---

## Godly

https://godly.design/

**Best for:** contemporary web design, unusual layouts, high-quality visual direction, motion-heavy work.

**AI usefulness:** `★★★☆☆`

Use primarily for:

- composition
- scale
- typography
- visual tension
- unusual navigation
- art direction

Do not blindly translate Godly-style sites into product UI. Many examples optimise for impact rather than usability.

---

## SiteInspire

https://www.siteinspire.com/

**Best for:** editorial web design, typography, portfolios, studios, restrained art direction.

**AI usefulness:** `★★★☆☆`

Often useful when we want something less trend-chasing than typical startup galleries.

---

## Land-book

https://land-book.com/

**Best for:** landing pages, product presentation, hero composition, marketing hierarchy.

**AI usefulness:** `★★★☆☆`

Useful for analysing:

- first-screen hierarchy
- CTA placement
- product storytelling
- image/text balance

---

## Layers

https://layers.to/

**Best for:** current visual trends, interface fragments, portfolio work, UI details.

**AI usefulness:** `★★★☆☆`

Good discovery source. Pair it with a more structured source before implementation.

---

## Are.na

https://www.are.na/

**Best for:** concept research, visual culture, obscure references, material studies, historical context.

**AI usefulness:** `★★★☆☆`

Are.na is especially valuable when we are building a **world** rather than searching for a component.

Use channels as mood / concept evidence, then describe which ideas matter.

---

## Brutalist Websites

https://brutalistwebsites.com/

**Best for:** raw layouts, anti-polish, typography, unconventional composition.

**AI usefulness:** `★★★☆☆`

Useful when the desired direction needs friction, restraint or deliberate awkwardness.

Do not treat brutality as an excuse for poor usability.

---

# 3. Design systems and component research

These are among the most useful sources for AI because they expose **rules + components + code + usage rationale**.

## The Component Gallery

https://component.gallery/

**AI usefulness:** `★★★★★`

A cross-design-system catalogue of common UI components.

Use it to compare how different systems solve the same component before inventing a new one.

Excellent for questions such as:

- what variants does a mature Date Picker need?
- how do systems handle empty states?
- what does a robust Alert component expose?

---

## Design Systems Repo

https://designsystemsrepo.com/

**AI usefulness:** `★★★★☆`

Curated directory of public design systems, guidelines, tools and articles.

Useful as a map for finding domain-specific systems rather than as a design system itself.

---

## DesignSystems.com

https://www.designsystems.com/

**AI usefulness:** `★★★★☆`

Useful for design-system process, governance, component thinking and real-world system architecture.

---

## shadcn/ui

https://ui.shadcn.com/

GitHub:
https://github.com/shadcn-ui/ui

**AI usefulness:** `★★★★★`

Particularly strong for agent workflows because the components are open code rather than opaque package internals.

Use as:

- implementation reference
- accessibility baseline
- component architecture reference
- starting material to reshape into our own visual language

**Important:** never let the default shadcn visual style become the project identity by accident.

Use the architecture, not the generic aesthetic.

---

## Radix UI

https://www.radix-ui.com/

**AI usefulness:** `★★★★★`

Excellent primitive layer for:

- behaviour
- accessibility
- state models
- keyboard interaction
- composable components

Very useful when we want to separate **interaction logic** from **visual design**.

---

## React Aria

https://react-spectrum.adobe.com/react-aria/

**AI usefulness:** `★★★★★`

Excellent reference for accessible interaction behaviour and complex controls.

Use it when we need to understand what a component must *do*, not what it should *look like*.

---

## Storybook

https://storybook.js.org/

**AI usefulness:** `★★★★★`

A good Storybook instance is one of the best inputs an AI agent can receive because it exposes:

- component variants
- props
- states
- edge cases
- documentation
- isolated interaction behaviour

For our own projects, a maintained Storybook can become part of the machine-readable design DNA.

---

# 4. Mature design systems worth studying

Use these when we want to understand **why** robust product systems make particular decisions.

## Apple Human Interface Guidelines

https://developer.apple.com/design/human-interface-guidelines/

**AI usefulness:** `★★★★★`

Best for interaction principles, platform behaviour, hierarchy and native patterns.

---

## Material Design 3

https://m3.material.io/

**AI usefulness:** `★★★★★`

Excellent documentation of tokens, states, accessibility, interaction and system logic.

Do not automatically inherit Material's visual identity.

---

## IBM Carbon

https://carbondesignsystem.com/

**AI usefulness:** `★★★★★`

Especially useful for dense, technical, enterprise and data-heavy interfaces.

Study the clarity and architecture without inheriting corporate visual weight.

---

## Shopify Polaris

https://polaris.shopify.com/

**AI usefulness:** `★★★★★`

Strong reference for commerce workflows, forms, merchant tools, content design and operational UX.

---

## Atlassian Design System

https://atlassian.design/

**AI usefulness:** `★★★★★`

Useful for complex application states, navigation, teamwork tools and dense functional UI.

---

# 5. Figma and collaborative design sources

## Figma Community

https://www.figma.com/community

**AI usefulness:** `★★★★★` when the actual Figma file is accessible through the Figma integration.

This is more valuable than a screenshot because the agent may be able to understand:

- component hierarchy
- variants
- frames
- spacing
- styles
- tokens
- layout relationships

When possible, provide the actual Figma file or component rather than an exported image.

---

## Figma design-system resources

https://www.designsystems.com/

The site includes links to several public design systems available in Figma.

Use these to inspect how professional teams map:

```text
Foundations
→ tokens
→ components
→ patterns
→ product screens
```

---

# 6. Creative coding / generative design

## p5.js

https://p5js.org/

**AI usefulness:** `★★★★★`

Excellent for rapid visual prototypes, generative systems, interaction experiments and visual sketches.

Because examples are code-based, an agent can both interpret and reproduce the underlying logic.

---

## Three.js

https://threejs.org/

**AI usefulness:** `★★★★★`

Use for:

- spatial interfaces
- 3D
- shaders
- particles
- generative environments
- unusual web interaction

The examples library is particularly valuable because each visual has corresponding implementation code.

---

## GSAP

https://gsap.com/

**AI usefulness:** `★★★★★`

Excellent for motion systems, scroll choreography, timelines and expressive web interaction.

Use motion as information and rhythm, not as decorative sugar.

---

## Motion

https://motion.dev/

**AI usefulness:** `★★★★★`

Good for production-friendly UI motion, gestures, layout transitions and interaction feedback.

---

## Codrops

https://tympanus.net/codrops/

**AI usefulness:** `★★★★☆`

A particularly useful bridge between experimental visual design and working front-end code.

Good source for:

- unconventional navigation
- typography experiments
- WebGL
- transitions
- shaders
- interaction concepts

---

# 7. Motion, animation and spatial tools

## Rive

https://rive.app/

**AI usefulness:** `★★★★☆`

Useful for interactive vector animation, state machines and UI animation that responds to application state.

Rive is particularly interesting when animation is **functional**, not merely cinematic.

---

## Spline

https://spline.design/

**AI usefulness:** `★★★★☆`

Useful for spatial sketches, 3D objects and interactive scenes.

Best used to communicate form and spatial behaviour rather than as a default visual effect.

---

## Framer

https://www.framer.com/

**AI usefulness:** `★★★★☆`

Useful for rapid web prototypes, responsive layout experiments and interactive design exploration.

---

## ProtoPie

https://www.protopie.io/

**AI usefulness:** `★★★★☆`

Strong for detailed interaction prototypes where timing, state and input behaviour matter.

---

# 8. Typography

## Fonts In Use

https://fontsinuse.com/

**AI usefulness:** `★★★★☆`

One of the best references because type is shown in actual cultural and design context rather than isolated specimens.

Use for:

- historical references
- editorial identity
- packaging
- signage
- unusual pairings

---

## Typewolf

https://www.typewolf.com/

**AI usefulness:** `★★★★☆`

Very useful for studying web typography and font pairings in context.

---

## Google Fonts Knowledge

https://fonts.google.com/knowledge

**AI usefulness:** `★★★★★`

Strong educational source for typography principles and terminology.

---

## Fontshare

https://www.fontshare.com/

**AI usefulness:** `★★★★☆`

High-quality free typefaces with clear specimens. Useful when a project needs an implementable font direction quickly.

---

## Velvetyne Type Foundry

https://velvetyne.fr/

**AI usefulness:** `★★★★☆`

Open-source, experimental typefaces. Good when the visual language needs more personality than standard product typography.

---

# 9. Branding and packaging

## The Dieline

https://thedieline.com/

**AI usefulness:** `★★★☆☆`

Excellent for packaging, material use, labelling, structure and retail presence.

When using it, identify whether the useful element is:

- package form
- label geometry
- print treatment
- typography
- transparency
- material
- shelf presence

---

## Brand New / UnderConsideration

https://www.underconsideration.com/brandnew/

**AI usefulness:** `★★★★☆`

Useful because projects are discussed and critiqued rather than merely displayed.

Good for understanding identity systems and the reasoning behind visual change.

---

## BP&O

https://bpando.org/

**AI usefulness:** `★★★★☆`

Strong source for branding, packaging and graphic identity with useful project context.

---

# 10. Colour and visual systems

## Realtime Colors

https://www.realtimecolors.com/

**AI usefulness:** `★★★★☆`

Useful for testing colour relationships in an interface context rather than viewing isolated swatches.

---

## OKLCH

https://oklch.com/

**AI usefulness:** `★★★★★`

Useful when constructing perceptually consistent colour scales for implementation.

---

## Adobe Color

https://color.adobe.com/

**AI usefulness:** `★★★★☆`

Useful for palette exploration and harmony studies.

---

# 11. Icons and small interface primitives

## Lucide

https://lucide.dev/

**AI usefulness:** `★★★★★`

Open, consistent and easy for coding agents to reference directly.

---

## Phosphor Icons

https://phosphoricons.com/

**AI usefulness:** `★★★★★`

Useful when a slightly warmer / more expressive icon family is needed.

---

## Iconoir

https://iconoir.com/

**AI usefulness:** `★★★★★`

Clean open-source icon set with a broad library.

---

# 12. Accessibility and interaction quality

## W3C Web Content Accessibility Guidelines

https://www.w3.org/WAI/standards-guidelines/wcag/

**AI usefulness:** `★★★★★`

Use as the authoritative baseline for web accessibility.

---

## Inclusive Components

https://inclusive-components.design/

**AI usefulness:** `★★★★★`

Excellent because accessibility is explained through real component behaviour and implementation decisions.

---

## The A11Y Project

https://www.a11yproject.com/

**AI usefulness:** `★★★★★`

Practical accessibility patterns, checklists and implementation guidance.

---

# 13. Toolset shortlist

These are tools worth keeping in the shared vocabulary because they allow us to move between intuition, prototype and implementation.

| Tool | Best role | Agent value |
|---|---|---|
| Figma | system design, layout, components | ★★★★★ |
| GitHub | code, design docs, versioned decisions | ★★★★★ |
| Storybook | machine-readable component catalogue | ★★★★★ |
| p5.js | visual sketching / generative ideas | ★★★★★ |
| Three.js | spatial and generative web | ★★★★★ |
| GSAP | expressive motion | ★★★★★ |
| Motion | product UI motion | ★★★★★ |
| Rive | stateful interactive animation | ★★★★☆ |
| Spline | rapid spatial / 3D concepts | ★★★★☆ |
| Framer | interactive responsive prototypes | ★★★★☆ |
| ProtoPie | behaviour-heavy prototypes | ★★★★☆ |

---

# 14. Sources that require more explanation

Some sources are visually excellent but relatively weak as raw AI input because they provide little structured context.

Examples include:

- Pinterest
- Instagram
- Behance moodboards
- random screenshot folders
- image-only inspiration feeds

These are still useful.

But when using them, add one or two sentences explaining **what you see**.

Example:

> Ignore the colours. I like how the typography ignores the container edges and how the product image occupies almost 70% of the composition.

That sentence can be more useful than another twenty screenshots.

---

# 15. Source capture template

When we discover a particularly valuable reference, add it here or to a project-specific reference file using this structure:

```text
## Source name

URL:

TYPE:
[design system / UI flow / typography / packaging / interaction / tool / etc]

WHY IT IS USEFUL:

AI READABILITY:
★★★★★

BORROW:
- ...
- ...

DO NOT BORROW:
- ...

BEST USED FOR:
- ...

NOTES:
- ...
```

---

# 16. Agent rule for this resource library

When an agent uses a source from this document:

1. inspect the source rather than relying only on its reputation
2. identify the exact design principle being borrowed
3. preserve the current project's approved Design DNA
4. prefer structural lessons over superficial copying
5. distinguish **interaction reference**, **visual reference**, **material reference**, and **implementation reference**
6. state uncertainty when the source cannot be inspected properly
7. never replace project-specific taste with the default aesthetic of a tool or component library

The purpose of this collection is not to make our work look like everyone else's.

It is to give us a richer visual vocabulary while keeping the final language our own.
