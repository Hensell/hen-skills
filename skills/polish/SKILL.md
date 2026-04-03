---
name: polish
description: Final ship pass for frontend work. Use to fix spacing, alignment, overflow, wrapping, interaction states, responsive edge cases, and low-level UX/UI inconsistencies.
argument-hint: [TARGET=<value>]
---

Polish is the last serious pass before shipping. It is where “good enough” becomes clean, resilient, and intentional.

Use `frontend-design` first for design principles. Use this skill only after the feature is functionally complete.

## What To Check

### Layout & Spacing

- Are spacing values consistent and token-driven?
- Do alignments feel exact, not approximate?
- Do dividers, headings, and content columns snap into a coherent rhythm?
- Is empty space deliberate rather than accidental?

### Typography

- Are line lengths controlled for reading?
- Are headings wrapping well?
- Do long titles or metadata strings break the layout?
- Are casing, tracking, and weights consistent?

### Responsive Stress

- Check narrow desktop, tablet, and mobile.
- Look for compressed rails, awkward wraps, and dead empty zones.
- Look for hidden overflow, clipped content, and uneven collapse behavior.
- If a composition only works at one width, it is not polished.

### Interaction States

- Default, hover, focus, active, disabled, loading, empty, success, error
- Touch targets large enough on mobile
- Clickable surfaces semantically correct
- Focus rings visible and intentional

### Surface Quality

- Borders, shadows, tinting, and backgrounds consistent
- Images keep aspect ratio and do not cause layout shift
- Icons align optically with text
- Copy sounds consistent across labels, buttons, and helper text

## Common Problems To Fix

- titles that should stay on one line but wrap awkwardly
- metadata rails too narrow to remain readable
- full-card click behavior implemented only on a nested text link
- mobile collapse that leaves giant voids or broken rhythm
- decorative motion that overwhelms the UI
- inconsistent section spacing after multiple redesign passes

## Execution

1. Inspect the most compressed layout widths first.
2. Fix structural issues before cosmetic ones.
3. Tighten typography and spacing.
4. Verify semantic interaction behavior.
5. Re-run checks and test the built output if applicable.

## Never

- polish before the structure is sound
- hide overflow instead of fixing the source
- keep brittle hero or rail layouts that break at medium widths
- let detail work introduce regressions

Polish succeeds when the UI stops drawing attention to mistakes.
