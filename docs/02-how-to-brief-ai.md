# 02 — How to brief AI

The goal is not to write a giant perfect prompt.

The goal is to communicate enough of the **design intent** that the agent can make good decisions without inventing a new visual language.

## The briefing order

Use this order whenever possible:

1. **World / feeling**
2. **User experience**
3. **Visual priorities**
4. **What must be preserved**
5. **What must not happen**
6. **References and why they matter**
7. **Concrete implementation constraints**

This order matters.

Starting with implementation details too early can cause an agent to optimise the wrong thing.

---

## 1. Describe the world first

Instead of:

> Make a modern dashboard with rounded cards.

Prefer:

> The interface should feel quiet, tactile and modular. It should feel closer to a creative instrument than enterprise software. The user should immediately understand where to look, but still discover small moments of character.

Useful questions:

- What kind of object / place / tool does this feel like?
- Is it calm or energetic?
- Precise or loose?
- Warm or clinical?
- Editorial or utilitarian?
- Familiar or slightly alien?
- Dense or spacious?

---

## 2. Describe the user's experience

Design vision is not only appearance.

Explain what should happen in the user's head.

Examples:

> The user should understand the next action without reading instructions.

> The interface should feel powerful, but never overwhelming.

> Advanced functionality should be discoverable rather than constantly visible.

> The user should feel that they are manipulating material directly, not filling in a form.

This gives the agent a reason for visual decisions.

---

## 3. State the hierarchy

Tell the agent what deserves attention.

Example:

> The waveform is the hero. Playback controls are secondary. File management should almost disappear until needed.

Or:

> The producer and the food are the hero. Platform mechanics should visually recede.

This is often more useful than specifying pixel values.

---

## 4. Define protected elements

If part of the design is already correct, say so explicitly.

Use language such as:

> Preserve exactly:
> - current typography
> - image scale
> - navigation structure
> - spacing rhythm
> - product-card architecture

Without this, an agent may interpret “improve” as “redesign”.

---

## 5. Say what it must NOT become

Negative constraints are extremely valuable.

Example:

> Keep it minimal, but do not let it become generic SaaS.
> No excessive card grid.
> No glossy gradients.
> No fake hardware.
> Do not reduce the personality just to make it cleaner.

Useful contrast pairs:

- minimal, not sterile
- playful, not childish
- experimental, not chaotic
- technical, not corporate
- retro, not nostalgic cosplay
- luxurious, not conventional luxury
- brutalist, not hostile
- futuristic, not glossy sci-fi
- organic, not rustic

---

## 6. Explain references, do not just attach them

Bad:

> Make it like this image.

Better:

> From this reference, borrow:
> - the oversized typography
> - the unusually generous negative space
> - the off-centre composition
>
> Do not borrow:
> - the colour palette
> - the logo treatment
> - the photography style

The agent should extract **principles**, not clone surfaces.

---

## 7. Use natural language first

Do not force yourself to speak like a designer or developer.

Statements like these are useful:

> This feels too polite.

> It has lost the tension.

> The controls feel pokey.

> It looks like someone put a dashboard template over the idea.

> The empty space feels accidental rather than composed.

> It needs to feel heavier / quieter / stranger / more physical.

The agent's job is to translate that intuition into design variables.

---

# A practical prompt shape

Use this when starting a design task:

```text
CONTEXT
What are we designing and for whom?

DESIGN INTENT
What should it feel like?
What kind of world does it belong to?

USER EXPERIENCE
What should the user understand / feel / do immediately?

VISUAL HIERARCHY
What is the hero?
What should recede?

PRESERVE
What is already correct and must not change?

AVOID
What must this never drift into?

REFERENCES
For each reference:
- what to borrow
- what not to borrow

CONSTRAINTS
Platform, responsiveness, accessibility, technical limitations, etc.

TASK
What exactly should be changed now?
```

---

# Fast conversational version

For everyday work, this can be much shorter:

```text
I want this to feel:
[3–6 words]

The most important thing is:
[primary experience / hierarchy]

Keep:
[approved elements]

Do not let it become:
[anti-patterns]

From the references, I like:
[specific qualities]

Change:
[current task]
```

That is enough to start.

The repository supplies the deeper context.
