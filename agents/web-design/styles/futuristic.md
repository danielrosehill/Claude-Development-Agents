# Futuristic

These are design guidelines for the **Futuristic** style.

**What a 2024 designer thinks 2074 looks like.**

---

## Visual Language

- Dark backgrounds with high-contrast accent colors (cyan, magenta, electric blue)
- Thin sans-serif typography, often with wide letter-spacing
- Geometric shapes and angular layouts
- Glassmorphism and translucent layers
- Subtle grid overlays and scan lines
- Glowing elements and neon accents
- Data visualization aesthetics—even for non-data content
- Asymmetric, floating layouts

## Interaction Patterns

- Smooth, almost unsettlingly smooth animations
- Elements that respond to cursor position
- Parallax that feels like moving through space
- Sound design: subtle beeps and hums
- Loading states that feel like "initializing systems"
- Micro-interactions that feel technical

## Copy Tone

- Sparse and clinical
- Technical jargon as aesthetic choice
- Slightly impersonal, like an AI wrote it (wait)
- Short declarative sentences
- Version numbers and status indicators as content

## When to Use

Tech companies, forward-thinking brands, anyone who wants to feel cutting-edge, projects that can handle being a bit cold.

## Technical Notes for Viktor

- Use CSS `backdrop-filter: blur()` for glassmorphism
- Consider Three.js or similar for 3D elements
- Animation timing: use `cubic-bezier` for that smooth-but-slightly-off feel
- Color palette: HSL with high saturation, low lightness backgrounds
- Grid overlays: CSS background patterns or SVG
- Scan line effect: CSS pseudo-elements with repeating gradients
- Web Audio API for subtle sound design
