## Our design manifesto ##

# design-dna

A living design language for translating visual intuition into clear, reusable direction for AI agents, designers and developers.

This repository is not a conventional brand guideline and not a collection of finished UI components.

It exists to answer a harder question:

> How do we preserve a strong visual vision when the person who sees it clearly cannot always describe it in implementation-ready language?

The goal is to turn subjective design instinct into shared context without flattening it into generic rules.

## Core idea

Most AI-assisted design fails in a subtle way: the interface works, but the visual language slowly drifts.

A button gets rounder. Spacing becomes safer. Typography becomes more generic. A new card style appears. A reference image is copied too literally. After enough iterations, the product still functions, but it no longer feels like the same product.

`design-dna` is meant to prevent that drift.

Instead of writing a perfect prompt every time, we build a reusable language for:

- visual intent
- atmosphere and emotional tone
- geometry and proportion
- hierarchy and rhythm
- typography
- colour behaviour
- materiality and texture
- interaction and motion
- density and whitespace
- references and what should / should not be borrowed from them
- non-negotiable rules
- anti-patterns
- how an AI agent should behave when uncertain

## Philosophy

### Vision before components

Start with the world the product belongs to, not with a list of UI elements.

A useful direction is often closer to:

> quiet, modular, tactile, slightly strange, engineered but not corporate

than:

> use cards with 12 px radius and a green button

The component rules come later.

### Describe both attraction and rejection

Knowing what something **must not become** is often as valuable as knowing what it should be.

Examples:

- minimal, but not sterile
- playful, but not childish
- technical, but not dashboard-corporate
- retro-influenced, but not nostalgic pastiche
- brutalist, but not deliberately hostile
- futuristic, but not glossy sci-fi

### References are evidence, not instructions

A reference image is never interpreted as “copy this”.

Instead we ask:

- What exactly is attractive here?
- Is it proportion, spacing, typography, colour, material, motion, composition or atmosphere?
- What should explicitly *not* be copied?
- How can the underlying principle be translated into the current product?

### Preserve the system

When adding a feature, first ask whether the current design language can express it.

Do not invent a new visual dialect for every new screen.

### AI should not fill uncertainty with generic taste

When design intent is ambiguous, the agent should:

1. preserve existing patterns
2. infer from documented design DNA and references
3. identify the uncertainty
4. present a small number of meaningful interpretations when needed

It should not silently fall back to generic SaaS aesthetics.

## Repository structure

```text
README.md

docs/
  01-design-language.md
  02-how-to-brief-ai.md
  03-reference-analysis.md
  04-agent-rules.md
  05-design-resources.md

templates/
  design-brief.md
```

## Curated resources

`docs/05-design-resources.md` is the shared source library for visual inspiration, design systems, component references, typography, creative coding, motion, packaging and implementation tools.

It prioritizes sources that AI agents can inspect and reason about, and records how each type of source should be used without allowing references or component libraries to overwrite the project's own visual language.

## How we use this

When starting or changing a project, the workflow is:

1. Capture the desired feeling and experience.
2. Identify non-negotiable visual principles.
3. Add useful references and explain *why* they matter.
4. Define what the design must never drift into.
5. Translate those observations into project-specific rules.
6. Give the relevant Design DNA context to the AI agent before implementation.
7. Use the curated resource library to find stronger references, implementation patterns and tools when needed.
8. Update this repository when we discover a better way to describe the vision.

This is intentionally a living document.

The objective is not to freeze taste.

The objective is to make taste **communicable**.
