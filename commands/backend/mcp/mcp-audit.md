Please audit the MCP server:

- Verify that it has correct and logical tool definitions. These should match the structure of the API as currently defined. If you find tools that are incorrect or which are no longer supp

orted by the current API structure, remove them. If you find that the MCP is missing tools that would enhance the MCP, add them. When considering whether new tools would enhance the API, co

nsider whether they woud be useful functions for a user to access via an AI agent interface. Not every single API function needs to be documented, but many will be useful.
- Consider, always, tool consolidation. The current state of AI engineering requires that users be strategic about what fucntions are provided as discrete tools versus parameters. 
- Try to rtionalise explicit tool definitions by nesting smaller functions as parameters of existing tools where possible.
- Finally: MCP servers should be HTTP streamable unless there is a compelling reason for them to be STDIO tools. If you find an SSE server, refactor as streamable HTTP.
