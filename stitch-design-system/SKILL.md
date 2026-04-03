---
name: stitch-design-system
description: Create Google Stitch-friendly DESIGN.md files that encode atmosphere, palette, typography, layout, motion, and anti-patterns for premium UI generation.
---

Use this skill when the user wants a `DESIGN.md` or equivalent design-system prompt for Google Stitch.

## Output Goal

Generate a concise design-system document that Stitch can interpret reliably.

It should define:

- visual atmosphere
- palette and accent rules
- typography stack and hierarchy
- layout principles
- component behavior
- motion philosophy
- anti-patterns to avoid

## Required Structure

1. visual theme and atmosphere
2. color system with exact values
3. typography rules
4. layout and spacing rules
5. component guidance
6. motion and interaction rules
7. responsive behavior
8. explicit banned patterns

## Guidance

- describe the system in natural language that an agent can execute
- keep the palette disciplined
- make anti-patterns explicit
- encode responsiveness and performance constraints, not just looks
- prefer one coherent design language over many options

If the user already has a strong visual direction, translate it. If not, derive one from the product context first.
