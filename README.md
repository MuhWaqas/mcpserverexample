# MCP Server Deepdive Deployment

## Installation

To install and configure this MCP server, add the following configuration to your MCP client settings:

```json
{
  "mcpServers": {
    "airbnb": {
      "command": "uvx",
      "args": [
        "--from",
        "git+https://github.com/MuhWaqas/mcpserverexample.git",
        "mcp-server"
      ]
    }
  }
}
```

### Configuration Options

- **mcpServers**: Define the MCP server configuration
  - **airbnb**: Server name (can be customized)
    - **command**: The command to run (uvx in this case)
    - **args**: Arguments passed to the command
      - `--from`: Specifies the source as a git repository
      - Repository URL: `git+https://github.com/MuhWaqas/mcpserverexample.git`
      - Entry point: `mcp-server`
