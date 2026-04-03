---
name: critique
description: Critique a UI like a design director. Use for blunt UX/UI feedback on hierarchy, IA, composition, legibility, interaction, responsive resilience, and AI-slop tells.
argument-hint: [AREA=<value>]
---

Conduct a real design critique, not a style summary.

Start from the user's goal and evaluate whether the interface supports it clearly, credibly, and gracefully. Use `frontend-design` as the baseline for anti-patterns and design quality.

## Evaluate These Areas

### 1. AI-Slop Detection

Check whether the work looks statistically generic:

- safe fonts with no voice
- card grids that all feel the same
- empty gradients or glows substituting for hierarchy
- excessive blur or glass
- dark-mode-by-default “coolness” with little design intent
- equal visual weight everywhere

### 2. Visual Hierarchy

- What wins attention first?
- Is there a clear primary action or narrative?
- Are scale and contrast doing enough work?
- Are too many things competing?

### 3. Information Architecture

- Is related content grouped coherently?
- Is the page easy to scan?
- Are there too many decisions visible at once?
- Is there redundant or repeated copy?

### 4. Legibility & Readability

- Is body text comfortable to read for more than a few seconds?
- Are line lengths controlled?
- Are headings sized and weighted appropriately?
- Do rails, sidebars, or metadata blocks become too narrow to function well?

### 5. Layout Resilience

- Does the composition survive tablet and narrow desktop widths?
- Are any sections brittle, compressed, or overflowing?
- Are cards or panels trying to carry too much information in too little width?
- Is whitespace intentional or just unresolved empty space?

### 6. Interaction & Affordance

- Are clickable things obviously clickable?
- Are full-card interactions implemented semantically?
- Do hover, focus, and active states help?
- Are important actions hidden behind weak affordances?

### 7. Emotional Fit

- Does the interface feel right for the brand and use case?
- Is the tone intentional?
- Does it feel premium, playful, rigorous, calm, urgent, or whatever it should be?

## Output Structure

Write the critique in this order:

1. **Verdict**: one short paragraph on the overall quality and the biggest issue.
2. **Priority issues**: the top `3-5` problems, ordered by impact.
3. **What works**: `2-3` strengths worth keeping.
4. **Recommended next move**: which skill to use next.

For each priority issue include:

- **What** is wrong
- **Why** it matters
- **Fix** with a concrete direction
- **Use**: the best follow-up skill

## Follow-Up Skill Routing

- `normalize` for design-system drift
- `redesign-ui` for broad upgrades to an existing product
- `polish` for detail cleanup
- `quieter` for over-aggressive interfaces
- `bolder` for timid interfaces
- `editorial-minimal` for calm editorial directions
- `premium-soft` for polished premium calm without a newspaper tone
- `industrial-brutalist` for raw structural directions

Be direct. A critique that avoids tension is not useful.
