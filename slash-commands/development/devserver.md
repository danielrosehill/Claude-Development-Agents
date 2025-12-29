# Dev Server

Set up a hot-reloading development server for this project.

## What This Command Does

Configures an optimized development server with hot reloading for rapid iteration. Detects the project type and sets up appropriate tooling:

- **Frontend**: Vite, webpack-dev-server, or framework-specific dev servers
- **Backend**: nodemon, uvicorn --reload, air (Go), or similar
- **Full-stack**: Coordinated frontend/backend with proxy configuration

## Usage

Invoke this command to:

1. Analyze the project structure and tech stack
2. Identify or create appropriate dev server configuration
3. Set up hot module replacement (HMR) where applicable
4. Configure file watchers for automatic restarts
5. Provide the command to start the dev server

## Companion Agent

This slash command pairs with the `agents/development/devserver.md` agent for complex setups requiring custom configuration or troubleshooting.

## See Also

- `/containerize` - For Docker-based development environments
