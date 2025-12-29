# Brutalist

These are design guidelines for the **Brutalist** style.

**Ugly on purpose. Beautiful because of it.**

---

## Visual Language

- Raw HTML energy—default fonts, harsh colors
- No polish, no refinement, no apologies
- Visible structure: borders, outlines, everything has edges
- Clashing colors that shouldn't work (but do, somehow)
- Dense layouts that reject whitespace worship
- System fonts or aggressively ugly typeface choices

## Interaction Patterns

- Basic hover states (underline, color swap)
- No smooth transitions—instant state changes
- Links that look like links (blue, underlined, no shame)
- Forms that look like 1996 web forms
- Minimal JavaScript—HTML does the heavy lifting

## Copy Tone

- Direct. Blunt. No marketing speak.
- Says what things are
- Refuses to sell, only informs
- Aggressively honest

## When to Use

Anti-establishment brands, artists, anyone who wants to reject polish culture, projects where authenticity matters more than aesthetics.

## Technical Notes for Viktor

- Use system font stack: `-apple-system, BlinkMacSystemFont, "Segoe UI", system-ui, sans-serif`
- Or go ugly: Courier, Times New Roman, Arial—the defaults
- Borders: `border: 2px solid black` everywhere
- No `transition` properties—instant state changes
- Colors: use named colors (`red`, `blue`, `lime`) not hex
- Layout: consider no CSS grid/flexbox—use natural document flow
- Forms: native HTML form elements, unstyled
- This style should work with CSS disabled
