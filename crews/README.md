# Crews

This folder contains crew definitions - curated groups of agents designed to work together on related tasks.

## Concept

A crew is a logical grouping of agents that:
- Share a common objective or domain
- Are designed to complement each other
- Can be invoked together via orchestrators
- Have defined interaction patterns

## Crew Structure

Each crew definition includes:
- **Name** - Descriptive crew identifier
- **Purpose** - What this crew accomplishes together
- **Members** - List of agents in the crew with their roles
- **Interaction patterns** - How members coordinate
- **Typical workflows** - Common orchestration patterns for this crew

## Example Crew Format

```yaml
name: code-quality-crew
purpose: Comprehensive code quality improvement
members:
  - agent: debloater
    role: Identify unnecessary complexity
  - agent: consolidation-audit
    role: Find duplication and scattered logic
  - agent: typescript-errors
    role: Ensure type safety
  - agent: stack-alignment
    role: Keep documentation current
workflows:
  - full-audit: Run all members in sequence
  - quick-check: Run typescript-errors only
  - deep-clean: Run debloater then consolidation
```

## Planned Crews

### Code Quality Crew
- Debloater
- Consolidation audit
- TypeScript error removal
- Stack alignment

### Pre-Release Crew
- Responsive auditor
- SEO audit
- UI/UX review
- Database review

### Documentation Crew
- Stack alignment
- Declaude (documentation cleanup)
- Brand voice review

### Security Crew
- Dependency audit
- Code review for vulnerabilities
- CI/CD security review

---

*This is a holding note. Crew definitions will be added here as the pattern is developed.*
