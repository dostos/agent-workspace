# MCP Server Configurations

Reusable MCP server configurations for common use cases.

## Usage

Merge these into your project's `.claude/settings.json` under `mcpServers`.

## Available Configs

- `servers/filesystem.json` - Local file access
- `servers/fetch.json` - Web fetching
- `servers/memory.json` - Persistent memory
- `servers/sequential-thinking.json` - Step-by-step reasoning
- `servers/context7.json` - Context management (Upstash)
- `servers/serena.json` - IDE assistant context (requires project path)

## Example

```json
{
  "mcpServers": {
    "filesystem": {
      "command": "npx",
      "args": ["-y", "@anthropic/mcp-server-filesystem", "/path/to/project"]
    }
  }
}
```
