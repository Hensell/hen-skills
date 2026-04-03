---
name: redesign-ui
description: Upgrade an existing website or app in place without rewriting it from scratch. Use when the user wants a current product to feel more premium, coherent, or less generic while preserving behavior.
argument-hint: [TARGET=<value>]
---

Redesign the existing product by improving what is already there.

Use this skill for live products, legacy screens, portfolios, marketing pages, and apps that already work but feel weak, generic, inconsistent, or unfinished.

## Sequence

1. **Scan**
   - Identify framework, styling approach, and current design patterns.
   - Find the strongest existing screens, components, and tokens worth preserving.

2. **Diagnose**
   - List the generic patterns, weak hierarchy, layout failures, and missing states.
   - Separate systemic problems from local ones.

3. **Choose the upgrade path**
   - keep and refine
   - restructure without rebrand
   - elevate with a stronger visual direction

4. **Fix in place**
   - preserve behavior and content truth
   - improve composition, readability, interactions, and responsiveness
   - replace weak patterns rather than stacking more decoration on top

5. **Verify**
   - check narrow widths, long content, hover/focus states, and performance-sensitive motion

## What To Improve

- typography with better hierarchy and width control
- surfaces and borders that communicate structure
- layout patterns that avoid generic equal-card rows
- clearer clickable behavior and stronger affordances
- calmer, more intentional motion
- real responsive behavior, not just scaled-down desktop
- AI-slop patterns such as generic gradients, glass everywhere, or empty visual tricks

## Guardrails

- Do not rewrite from scratch unless the user explicitly wants that.
- Do not invent new product claims or fake content.
- Do not destroy a working IA in pursuit of visual novelty.
- Do not apply the same “premium” recipe to every project.

## Skill Routing

- Use `normalize` if the goal is consistency with an existing design system.
- Use `editorial-minimal`, `premium-soft`, or `industrial-brutalist` if the user wants a specific strong aesthetic.
- Use `polish` after the redesign is structurally complete.
