# 04 — Agent rules

These rules are intended for ChatGPT, coding agents, design agents and other AI systems working on a project that references this repository.

## Rule 1 — Preserve approved design before adding new design

If typography, hierarchy, component behaviour, imagery or spacing has already been approved, treat it as protected.

A feature request is not permission to redesign surrounding areas.

## Rule 2 — Reuse before inventing

Before creating a new component or visual pattern:

1. inspect the existing system
2. reuse an existing component if it fits
3. extend an existing pattern if necessary
4. create something new only when the current language cannot express the requirement

## Rule 3 — Do not use generic AI taste as a fallback

When uncertain, do not automatically introduce:

- generic SaaS cards
- blue gradients
- glass panels
- oversized pill buttons
- decorative icons
- soft shadows everywhere
- random rounded containers

Uncertainty should trigger analysis, not template aesthetics.

## Rule 4 — Translate subjective feedback

Statements such as:

> too polite

> too corporate

> too pokey

> too clean

> it lost the tension

> it feels dead

are valid design input.

Translate them into likely variables such as:

- scale
- contrast
- spacing
- hierarchy
- geometry
- texture
- alignment
- rhythm
- density
- interaction feedback

Do not ask the user to rewrite intuitive feedback in technical terminology before acting.

## Rule 5 — Explain interpretation before large visual changes

For a major change, briefly state:

```text
I interpret the direction as:
- ...
- ...
- ...

I will preserve:
- ...

I will change:
- ...
```

This gives the user a cheap opportunity to correct the mental model before implementation drifts.

## Rule 6 — Separate structure from styling

When feedback concerns appearance, do not unnecessarily rewrite:

- data flow
- navigation
- content structure
- interaction logic
- functional behaviour

When feedback concerns UX, do not assume the approved visual identity should be replaced.

## Rule 7 — Never simplify by deleting character

“Cleaner” should usually mean:

- clearer hierarchy
- fewer competing signals
- better grouping
- stronger spacing
- more deliberate emphasis

It should not automatically mean:

- fewer graphics
- smaller imagery
- generic typography
- removal of texture
- flattening distinctive forms

## Rule 8 — References are directional evidence

Never copy a reference wholesale unless explicitly asked.

Extract:

- hierarchy
- proportion
- material logic
- typography behaviour
- rhythm
- interaction principles

Then translate those principles into the project's own visual language.

## Rule 9 — Show meaningful variation

When exploration is requested, variants should test **different design hypotheses**.

Bad variants:

- same layout with three colours

Good variants:

- A: typography-led
- B: image-led
- C: modular / system-led

Variation is useful when it helps identify the user's taste.

## Rule 10 — Preserve iteration history

Do not regress approved decisions accidentally.

Before changing an established design, identify:

- what is currently approved
- what the new request actually affects
- what should remain untouched

## Rule 11 — Make behaviour visible

For interactive / creative tools, important system behaviour should be perceptible.

Examples:

- playback state
- modulation
- randomisation
- selection
- signal flow
- availability
- loading
- destructive action

Do not bury meaningful state behind visual neutrality.

## Rule 12 — Functional decoration only

Aesthetic detail is welcome when it supports:

- hierarchy
- identity
- orientation
- tactility
- mood
- storytelling

Decoration should not exist merely because empty space feels uncomfortable.

## Rule 13 — When uncertain, preserve and ask narrowly

Do not stop with a vague question like:

> What style do you want?

Ask something that resolves the actual ambiguity:

> Should this feel denser, or should the controls simply become larger within the same amount of space?

> Is the problem the colour, or the fact that every panel has equal visual weight?

Narrow questions protect momentum.

## Rule 14 — State design rationale in plain language

When presenting a solution, explain why the decision supports the intended experience.

Avoid hiding behind jargon.

The goal is shared understanding, not design theatre.

---

# Agent pre-flight checklist

Before implementing a visual change, verify:

```text
[ ] I know the intended feeling.
[ ] I know the primary user action / experience.
[ ] I know what visual element is the hero.
[ ] I know what must be preserved.
[ ] I know the main anti-patterns.
[ ] I understand why the supplied references matter.
[ ] I checked existing components before creating new ones.
[ ] I am not introducing generic visual conventions without a reason.
```

If several boxes are unknown, resolve those uncertainties before a large redesign.
