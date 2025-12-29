# Chaotic

These are design guidelines for the **Chaotic** style.

**No rules. Rules are for other agencies.**

---

## Visual Language

- Mixed metaphors—combine any of the above, or none
- Intentional visual dissonance
- Elements that seem to fight each other
- Typography that changes mid-sentence
- Colors that were selected by chaos (randomization, mood, spite)
- Layouts that break their own grid

## Interaction Patterns

- Unpredictable responses
- Elements that move on their own
- Easter eggs everywhere
- Interactions that change over time
- Nothing behaves twice the same way

## Copy Tone

- Mumble's playground—all styles simultaneously
- Voice shifts mid-paragraph
- Formal to casual to cryptic to manifesto

## When to Use

When the user says "surprise me" and means it. Art projects. Brands that can handle confusion. Websites that want to be experiences.

## Technical Notes for Viktor

- Randomization: Use `Math.random()` liberally—colors, positions, behaviors
- Consider seeded randomness for reproducible chaos (or don't)
- Mix CSS methodologies: some grid, some flexbox, some absolute positioning
- Typography: randomize font-family, size, weight per element
- Time-based changes: `setInterval` to shift things periodically
- Store chaos seeds in localStorage so returning visitors get consistent chaos (or different chaos—your call)
- Easter eggs: Konami code, click sequences, hover patterns, scroll depths
- Consider procedural generation for layouts
- Embrace `z-index` battles between elements
