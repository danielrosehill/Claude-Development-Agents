# Debug

Focus on diagnosing and fixing a single specific bug.

## What This Command Does

Invokes a focused debugging workflow for one bug at a time. This is not a general code review - it's laser-focused on:

1. Understanding the exact bug and its symptoms
2. Creating a minimal reproduction case
3. Diagnosing the root cause
4. Implementing the smallest fix that resolves it
5. Validating the fix with tests

## Usage

Invoke this command and provide:
- Description of the bug and observed behavior
- Expected behavior
- Reproduction steps (if known)
- Any relevant error messages or logs

## Companion Agent

This slash command pairs with the `agents/subdevelopers/debugging.md` agent for extended debugging sessions that require autonomous investigation.

## Key Principles

- Single-bug focus - don't expand scope to other issues
- Minimal change surface - smallest fix that works
- Evidence-driven - repro before fix, validate after
- If new bugs are discovered, note them but don't tackle them
