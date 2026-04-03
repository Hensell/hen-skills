---
name: normalize
description: Bring a feature back into alignment with the existing design system. Use when the product already has patterns and the goal is consistency, not a rebrand.
argument-hint: [FEATURE=<value>]
---

Normalize the feature so it feels native to the product.

Use this skill when the right answer is consistency with an existing system. If the user wants a larger visual upgrade or wants to make an existing product feel premium, use `redesign-ui` instead.

## What To Learn First

1. Find the design system, component library, tokens, and recurring patterns.
2. Identify which screens already represent the best version of the product.
3. Check whether the current feature is off because of styling drift, one-off components, or conceptual mismatch.

Do not guess at design system principles when the codebase can answer them.

## What Normalization Means

- Reuse existing components instead of inventing new ones.
- Replace hard-coded values with system tokens.
- Match typography, spacing, border treatment, color, and motion to the established product language.
- Bring interaction patterns back in line with the rest of the app.
- Preserve the existing product personality.

## Execution

Work through these areas:

- **Structure**: align layout with the product grid and spacing rhythm
- **Typography**: match weights, sizes, line lengths, and casing patterns
- **Surfaces**: reuse tokens for borders, backgrounds, elevation, and accents
- **Components**: prefer shared components and system variants
- **Interactions**: match focus, hover, active, empty, loading, and error behavior
- **Responsive behavior**: match breakpoints and collapse patterns used elsewhere
- **Accessibility**: preserve contrast, focus visibility, semantics, and keyboard behavior

## Guardrails

- Do not introduce a new visual language.
- Do not treat “cleaner” as automatically “more consistent.”
- Do not add flair that the rest of the product does not support.
- Do not keep one-off code if it should become reusable.

## Clean Up

- Remove obsolete styles and dead variants.
- Consolidate duplicated patterns into shared primitives where appropriate.
- Run the relevant checks for linting, typing, testing, and visual regressions.

Normalization succeeds when the user stops noticing the feature as a special case.
