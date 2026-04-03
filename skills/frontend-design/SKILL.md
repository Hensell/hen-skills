---
name: frontend-design
description: Design and implement distinctive, production-grade frontend interfaces for new features or major visual work. Use when building pages, components, or strong UI directions that should avoid generic AI aesthetics.
license: Apache 2.0. Based on Anthropic's frontend-design skill. See NOTICE.md for attribution.
---

Create frontend work that feels designed, not merely assembled.

Use this skill for new UI, major visual changes, and any task where design quality matters. If the user wants to upgrade an existing product without rewriting it, also consider `redesign-ui`. If they want a very specific aesthetic, prefer a preset skill such as `editorial-minimal`, `premium-soft`, or `industrial-brutalist`.

## Design Dials

Choose the dials before writing code. Defaults: `variance 7`, `motion 5`, `density 4`.

- **Variance**: How asymmetrical or surprising the composition should be.
- **Motion**: How choreographed or restrained the interactions should feel.
- **Density**: How airy vs. information-rich the screen should be.

Do not ask the user to provide numbers unless they already think that way. Infer the dial settings from the prompt and product context.

## Working Order

1. Read the product context and the existing codebase first.
2. Pick one clear visual direction and one memorable device.
3. Decide what must be static, what must be interactive, and what can be removed.
4. Implement real code, not mockup-like scaffolding.
5. Check responsiveness, overflow, motion, and accessibility before stopping.

## Core Principles

- Commit to a strong point of view. Refined minimalism and bold maximalism can both work; indecision does not.
- Hierarchy matters more than decoration.
- Use fewer, better ideas. One strong compositional move beats five weak ones.
- Match the design to the product. A portfolio can be more expressive than a finance tool.
- Preserve usability under all aesthetic choices.

## Typography

- Pair a distinctive display face with a readable body face.
- Use fluid sizing with `clamp()` for headlines and key text.
- Create real hierarchy with size, weight, width, spacing, and line height.
- Keep body text readable: usually `45-75` characters per line.
- Use `text-wrap: balance` or `pretty` for short headings when supported.
- Use monospace intentionally for metadata, labels, or technical readouts, not as a lazy product identity.

Never default to:
- `Inter`, `Roboto`, `Arial`, or similar safe defaults for premium work
- giant all-caps everywhere
- identical heading scales across sections

## Color & Surface

- Build around a disciplined neutral base and a single clear accent.
- Tint neutrals toward the project hue; avoid dead gray everywhere.
- Prefer `oklch` or `color-mix()` when the stack supports it.
- Use color to communicate priority, action, state, or structure.
- If a section feels flat, add depth with subtle texture, image treatment, or controlled atmosphere, not random gradients.

Never default to:
- cyan/purple AI gradients
- neon-on-dark as a generic shortcut
- pure black or pure white
- glassmorphism as a blanket solution

## Layout & Composition

- Use CSS Grid when the structure matters. Do not do complex percentage math in flexbox when grid is clearer.
- Create rhythm with varied spacing and sectional contrast.
- Break symmetry intentionally, not accidentally.
- Use containment well: long-reading blocks need width control, data views need alignment, hero areas need a focal anchor.
- Treat whitespace as a structural tool, not leftover room.

Avoid:
- three equal feature cards by default
- nesting cards inside cards without a strong reason
- centering every section
- layouts that collapse into messy wraps at medium widths

## Interaction & Motion

- Motion must clarify state, hierarchy, or sequencing.
- Use `transform` and `opacity` for animation. Avoid layout-thrashing properties.
- Respect `prefers-reduced-motion`.
- Keep hover/focus/active states intentional and visible.
- Make tappable/clickable surfaces obvious. If a whole card behaves like a link, make the whole card a link.

Avoid:
- bounce or elastic easing for premium interfaces
- decorative blur on large scrolling surfaces
- hiding key affordances inside hover-only patterns

## Reliability Guardrails

- Do not use `h-screen` for critical full-height sections; prefer `min-height: 100dvh`.
- Collapse asymmetrical layouts aggressively below tablet widths.
- Test long titles, long tags, long metadata, and narrow containers.
- Prevent horizontal overflow by design, not with `overflow-x: hidden` band-aids.
- Do not create beautiful but brittle compositions.
- Keep z-index usage deliberate and systemic.

## Anti-Slop Checklist

If the output would make someone say “this looks AI-generated,” stop and correct course.

Common tells:
- identical card grids
- generic gradients
- dark background plus glow plus blur
- typography with no character
- decorative metrics or badges everywhere
- every button styled as primary
- layout that looks equally weighted from top to bottom

## Preset Routing

Use these when the prompt clearly calls for them:

- **`editorial-minimal`**: newspaper, warm editorial, calm luxury, portfolio writing surfaces
- **`premium-soft`**: polished premium softness, airy consumer surfaces, calm modern product marketing
- **`industrial-brutalist`**: raw Swiss grids, tactical telemetry, harsh utilitarian structure
- **`redesign-ui`**: improve an existing site or app in place instead of designing from scratch

## Final Check

Before finishing:

- Is there one clear focal point?
- Does the layout still work at tablet widths?
- Are the clickable areas obvious?
- Is body text pleasant to read?
- Does the design feel intentional rather than fashionable?
- Does the code reflect the design system instead of one-off improvisation?

Deliver code that is production-grade, memorable, and structurally sound.
