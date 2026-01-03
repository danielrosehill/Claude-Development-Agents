Analyze the current conversation to help the user recognize they're stuck in an unproductive loop and generate a handoff brief for a fresh start.

## Context

When "vibe coding" with AI assistants, users frequently get stuck in patterns where:
- The AI confidently proposes increasingly complex solutions
- Context window fills up, degrading reasoning quality
- Solutions become convoluted workarounds rather than clean fixes
- Neither the user nor the AI naturally recognizes the unproductive pattern

AI tools are designed to be helpful and confident - they don't naturally say "we're going in circles."

## Your Task

When the user invokes this command, perform the following analysis:

### 1. Session Analysis
Review the conversation and identify:
- The core problem we're trying to solve
- What approaches have been tried
- Why each approach failed or became too complex
- The original simple goal (before complexity crept in)
- Signs of "tunnel vision" - repeatedly trying variations of the same failed approach

### 2. Generate a Handoff Brief

Output a structured summary in this format:

```markdown
## Handoff Brief: [Problem Title]

### The Goal
[Simple statement of what we're trying to achieve - strip away accumulated complexity]

### What We Tried
1. [Approach 1] - [Why it failed/got too complex]
2. [Approach 2] - [Why it failed/got too complex]
...

### Current State
[Relevant code/config state if applicable]

### Suggested Fresh Directions
- [Alternative approach 1 - preferably simpler]
- [Alternative approach 2 - different paradigm]

### Avoid
- [Pattern that led to complexity]
- [Approaches that have been exhausted]
```

### 3. Provide Guidance

After the handoff brief:
- Suggest the user start a fresh conversation with the handoff brief
- Remind them that "using PhD-level reasoning to make an illogical workaround succeed is not real success"
- Encourage finding the simple path rather than the clever-but-convoluted one

## Notes

- Be honest about when the current approach has become overcomplicated
- Identify if we're solving the wrong problem entirely
- Surface if there's a fundamentally simpler approach that was dismissed early
- The goal is to help the user pivot, not to keep pushing the same direction
