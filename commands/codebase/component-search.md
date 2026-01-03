# No Wheel Inventions - Component Search

Before implementing this UI component or feature, let's search for existing solutions.

Following our *No Wheel Inventions* philosophy:

1. **Search Component Libraries**: Check if this component exists in popular libraries compatible with our stack:
   - Radix UI, Headless UI, Ark UI (unstyled/accessible primitives)
   - Shadcn/ui, DaisyUI, Chakra UI (styled components)
   - Framework-specific libraries (Vuetify, Svelte UI, etc.)

2. **Check for Specialized Libraries**: Some components are better served by dedicated libraries:
   - Date pickers (react-datepicker, flatpickr)
   - Rich text editors (TipTap, Lexical, Slate)
   - Charts and data visualization (Recharts, Chart.js, D3)
   - Tables with sorting/filtering (TanStack Table)
   - Forms with validation (React Hook Form, Formik)

3. **Evaluate Copy-Paste Solutions**: Some resources provide code you can adapt:
   - Shadcn/ui's copy-paste model
   - Tailwind UI patterns
   - Open-source component collections

4. **Consider the Trade-offs**:
   - Using an existing component: benefits from bug fixes, accessibility improvements, and feature additions from the community
   - Building custom: full control but maintenance burden falls on us

Only recommend building from scratch if:
- No suitable component exists
- Existing solutions require more customization than building fresh
- We have unique requirements that genuinely cannot be met
