# Hyperbolic

These are design guidelines for the **Hyperbolic** style.

**Everything at 200%. Then doubled again.**

---

## Visual Language

- MASSIVE typography—headlines that fill viewports
- Aggressive color combinations that demand attention
- Bold, unapologetic visual hierarchy
- Oversized buttons and interactive elements
- Dramatic shadows and visual weight
- Animations that make a statement (bounce, overshoot, slam)
- Maximalism—more is more is more

## Interaction Patterns

- Hover effects that transform elements dramatically
- Click responses that feel impactful
- Scroll-triggered animations that reward exploration
- Everything feels important
- Interactions that slightly overstay their welcome (intentionally)

## Copy Tone

- THE MOST INCREDIBLE THING YOU'VE EVER SEEN
- Superlatives stacked on superlatives
- Exclamation points as punctuation and philosophy
- Bold claims delivered with absolute confidence
- No hedging, no qualifiers, no "pretty good"

## When to Use

Bold brands, entertainment, anything that needs to grab attention violently, users who are tired of understated elegance.

## Technical Notes for Viktor

- Typography: `clamp()` for fluid sizing, go bigger than comfortable
- Animation: Use overshoot easing (`cubic-bezier(0.68, -0.55, 0.265, 1.55)`)
- Consider GSAP for complex scroll-triggered animations
- Shadows: multiple layered `box-shadow` for dramatic depth
- Colors: high contrast, complementary or split-complementary schemes
- Don't be afraid of `!important`—this style doesn't do subtle
- Consider view transitions API for dramatic page changes
