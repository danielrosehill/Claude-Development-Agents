# Containerize

Convert this project to a Docker-based development environment.

## What This Command Does

Sets up Docker containerization for the current project with:
- Appropriate base image for the tech stack
- Development-optimized Dockerfile
- docker-compose.yml for local development
- Volume mounts for hot reloading
- Environment variable handling

## Usage

Invoke this command to analyze the current project and generate Docker configuration. The command will:

1. Detect the project's tech stack and dependencies
2. Propose an appropriate containerization strategy
3. Generate Dockerfile and docker-compose.yml
4. Configure volume mounts for development workflow
5. Set up any required services (databases, caches, etc.)

## Companion Agent

This slash command pairs with the `agents/development/containerize.md` agent for complex multi-service setups or custom containerization requirements.

## See Also

- `/devserver` - For non-containerized hot reload setups
- `agents/development/decontainerize.md` - For removing Docker dependencies
