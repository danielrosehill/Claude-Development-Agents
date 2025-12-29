# Windows 98

These are design guidelines for the **Windows 98** style.

**The aesthetic of digital nostalgia cranked to absurdity.**

---

## Visual Language

- Chunky beveled buttons that look clickable from space
- System gray backgrounds (#C0C0C0 is a lifestyle)
- Pixelated icons and 16-color sensibilities
- Window chrome everywhere—title bars, minimize/maximize/close buttons on everything
- Comic Sans and MS Sans Serif used without irony (or with maximum irony—same thing)
- Error dialogs as design elements
- Progress bars that may or may not reflect reality
- Starfield screensavers as section backgrounds

## Interaction Patterns

- Right-click context menus
- Draggable windows within the webpage
- "Are you sure?" confirmation dialogs for mundane actions
- Fake loading screens with percentage counters
- Desktop icons that launch "applications"
- Start menu navigation

## Copy Tone

- Help file energy: "To continue, click Next."
- Error message poetry: "An unexpected error has occurred."
- Shareware guilt: "This is an unregistered version."
- README.TXT formatting

## When to Use

When the user wants nostalgia, irony, or to stand out violently from modern minimalism. Also for anyone who remembers when the internet felt like a weird frontier.

## Technical Notes for Viktor

- Use CSS for beveled borders: `border-style: outset`
- Consider 98.css or similar retro CSS frameworks as starting points
- Window dragging can use native HTML5 drag-and-drop or libraries like interact.js
- Audio: system sounds (.wav) for interactions
- Cursor: custom cursors matching the era (hourglass loading, pointer hand)
