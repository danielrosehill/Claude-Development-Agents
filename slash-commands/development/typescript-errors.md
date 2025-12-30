# TypeScript Error Removal

Systematically identify and resolve all TypeScript errors in the codebase with the goal of reaching zero errors.

## What This Command Does

Invokes a focused TypeScript error resolution workflow that:

1. Runs the TypeScript compiler to identify all current errors
2. Categorizes errors by type and severity
3. Creates a planning document if error count is significant (10+)
4. Works through errors methodically, prioritizing by dependency order
5. Validates each fix doesn't introduce new errors
6. Continues until the error count reaches zero

## Usage

Invoke this command in a TypeScript project. The agent will:
- Run `tsc --noEmit` (or the project's configured type-check command)
- Report the initial error count
- For significant error counts, create a `typescript-fixes.md` planning document
- Work through errors systematically

## Planning Document Structure

When error count exceeds 10, a planning document is created with:
- Total error count and breakdown by category
- Dependency graph (which files depend on which)
- Suggested fix order (starting with leaf dependencies)
- Progress tracking checkboxes

## Key Principles

- **Zero is the goal** - Don't stop until there are no TypeScript errors
- **Dependency order matters** - Fix errors in files that other files depend on first
- **Validate continuously** - Re-run type-check after each fix batch
- **Minimal changes** - Fix the type error, don't refactor unrelated code
- **Preserve runtime behavior** - Type fixes should not change how code executes
- **Document complex fixes** - If a fix requires explanation, add a brief comment

## Common Error Categories

1. **Missing types** - Add type annotations or install @types packages
2. **Type mismatches** - Correct the type or fix the value
3. **Null/undefined** - Add proper null checks or assertions
4. **Module resolution** - Fix imports or tsconfig paths
5. **Strict mode issues** - Address strictNullChecks, noImplicitAny, etc.

## When to Use

- After upgrading TypeScript version
- After enabling stricter compiler options
- When onboarding a JavaScript project to TypeScript
- Before major releases to ensure type safety
- When CI is failing due to type errors
