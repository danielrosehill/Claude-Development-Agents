# Claude Development Agents

A collection of Claude Code configurations for development workflows. Consolidates sub-agents, slash commands, and prompt snippets developed over the past few months.

## Taxonomy

### Agents (`/agents/`)

Full autonomous agent configurations for complex, multi-step tasks. Agents work independently within defined scopes and have YAML frontmatter with metadata.

**Use when:** The task requires autonomous investigation, multiple steps, or extended workflows.

### Slash Commands (`/slash-commands/`)

Invokable commands that trigger specific workflows. Lighter than agents, designed for quick access to common operations.

**Use when:** You need to quickly invoke a focused workflow with `/command-name`.

### Snippets (`/snippets/`)

Paste-able prompt fragments for steering conversations. Not invoked as commands - simply copied into prompts to redirect AI behavior.

**Use when:** You need to inject context or redirect an ongoing conversation without starting a formal workflow.

## Directory Structure

```
agents/
  code-editing/        # Code manipulation and cleanup
  deployment/          # CI/CD and deployment automation
  development/         # Containerization, dev servers, stack integration
  github/              # Backups, forks, licensing, collaboration
  ides/                # IDE integrations
  stylistic/           # Writing style enforcement
  subdevelopers/       # Single-bug debugging, feature additions
  web-design/          # Multi-agent creative web design system
  web-development/     # Responsive auditing, AI SEO, frontend optimization

slash-commands/
  codebase/            # Component search, dependency audit, consolidation
  development/         # Containerize, debug, devserver, backup
  reviews/             # Stack, database, UI/UX, SEO, social, brand reviews
  workflow/            # Stuck handoffs, retrospectives, starting instructions

snippets/
  advisory/            # Smarter approach, right tool, efficiency checks
  complexity/          # Scope control, simplification requests
  debugging/           # Root cause focus, fire prevention
  session/             # Fresh starts, loop detection, corrections
  style/               # Emoji, docs, naming, structure preferences

private/
  new-configs/         # Staging area for new configurations
```

## Agent Categories

| Category | Purpose |
|----------|---------|
| code-editing | Comment removal, code cleanup |
| deployment | CI/CD setup, packaging, shipping |
| development | Containerization, dev servers, stack advising |
| github | Backups, forks, licensing, collaboration |
| ides | VS Code extensions and IDE tooling |
| stylistic | Writing style enforcement (declaude) |
| subdevelopers | Single-bug debugging, feature additions |
| web-design | Multi-agent creative web design system |
| web-development | Responsive auditing, AI SEO, frontend optimization |

## Slash Commands

### Development (`/slash-commands/development/`)

| Command | Purpose | Companion Agent |
|---------|---------|-----------------|
| `/backup` | Quick repository backup | `github/backup-repo.md` |
| `/containerize` | Docker setup | `development/containerize.md` |
| `/debug` | Focused bug fixing | `subdevelopers/debugging.md` |
| `/devserver` | Hot-reload setup | `development/devserver.md` |

### Reviews (`/slash-commands/reviews/`)

Advisory commands that ask "how can we do this better?":

| Command | Purpose |
|---------|---------|
| `/brand-voice` | Review copy against brand voice guidelines |
| `/database-review` | Database optimization, indexes, relationships |
| `/framework-leverage` | Are we fully using our framework's capabilities? |
| `/seo-audit` | Meta tags, sitemap, robots.txt, structured data |
| `/social-preview` | Open Graph tags, Twitter cards, platform previews |
| `/stack-review` | Fresh eyes on technology stack choices |
| `/ui-ux-review` | CSS efficiency and UX improvements |

### Codebase (`/slash-commands/codebase/`)

| Command | Purpose |
|---------|---------|
| `/component-search` | Find existing UI components |
| `/consolidate` | Find consolidation opportunities and inefficiencies |
| `/dependency-audit` | Audit underutilized packages |
| `/search-upgrade` | Evaluate search strategies (fuzzy, vector, full-text) |
| `/template-check` | Find existing templates |

### Workflow (`/slash-commands/workflow/`)

| Command | Purpose |
|---------|---------|
| `/retrospective` | Review for wheel reinvention |
| `/starting-instruction` | No wheel inventions reminder |
| `/stuck` | Generate handoff brief when stuck |

## Snippets

### Session Control (`/snippets/session/`)
- `fresh-perspective` - Request first-principles approach
- `previous-session-unhelpful` - Context for retrying after failed session
- `this-was-the-issue` - Correct a misdiagnosis
- `went-in-circles` - Redirect when stuck in loops
- `wrong-direction` - Signal need for pivot

### Complexity Control (`/snippets/complexity/`)
- `stop-expanding-scope` - Prevent scope creep
- `too-complex` - Pull back from overcomplicated solutions

### Debugging Focus (`/snippets/debugging/`)
- `dont-put-out-fires` - Focus on fundamental problems
- `find-root-cause` - Push past symptom-fixing

### Style Directives (`/snippets/style/`)
- `balanced-structure` - Prevent fragmented documents
- `match-brand-voice` - Enforce specific brand voice
- `minimal-docs` - Prevent over-documentation
- `no-all-caps` - Enforce kebab-case naming
- `no-emojis` - Prohibit emoji usage

### Advisory Mode (`/snippets/advisory/`)
- `advisor-mode` - Switch to advisory rather than executor mode
- `efficiency-check` - Request efficiency analysis
- `hidden-relationships` - Identify untapped data relationships
- `native-solution` - Check if framework already solves this
- `right-tool` - Question if we're using the right tool
- `smarter-approach` - Ask "how can we do this smarter?"

## Workflow

New configurations are drafted in `private/new-configs/` and processed via the `/sort` command, which validates and moves them to appropriate categories.

## Philosophy

This toolkit emphasizes:
- **No Wheel Inventions** - Leverage existing solutions before building custom
- **Focused Scope** - Each tool does one thing well
- **Fresh Starts** - Recognize when to pivot rather than persist
- **Root Cause Thinking** - Fix problems, not symptoms
- **Advisory Over Execution** - Use AI as a strategic guide, not just a task executor
