# Orchestrators

This folder contains orchestrator configurations that coordinate multiple agents in sequence or parallel.

## Concept

Orchestrators are meta-agents that:
- Invoke multiple agents in a defined order
- Pass context between agent stages
- Handle transitions and handoffs
- Aggregate results from multiple agents

## Structure

Each orchestrator defines:
- **Agents to invoke** - Which agents participate
- **Execution order** - Sequential, parallel, or conditional
- **Data flow** - How output from one agent feeds into the next
- **Completion criteria** - When the orchestrated workflow is done

## Relationship to Crews

- **Orchestrators** define HOW agents work together (the workflow)
- **Crews** define WHICH agents work together (the team composition)

An orchestrator might reference a crew, or define its own agent list inline.

## Implementation Status

This folder is a placeholder for future orchestrator configurations. The orchestration pattern will enable complex multi-agent workflows invoked via single slash commands.

## Planned Orchestrators

- `code-quality-review` - Runs debloater, consolidation, type checking in sequence
- `pre-release-audit` - Comprehensive checks before shipping
- `onboarding-setup` - Stack alignment, documentation, environment setup

---

*This is a holding note. Orchestrator configurations will be added here as the pattern is developed.*
