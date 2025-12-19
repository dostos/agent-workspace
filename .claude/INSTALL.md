# Claude Code Installation

## As Submodule

1. Add to your project:
   ```bash
   git submodule add <repo-url> .agent-workspace
   ```

2. Create symlink or copy CLAUDE.md to project root:
   ```bash
   ln -s .agent-workspace/CLAUDE.md CLAUDE.md
   ```

## Skills Registration

Add to your `.claude/settings.json`:

```json
{
  "skills": [
    {
      "name": "commit",
      "description": "Create module-prefixed conventional commit",
      "command": "cat .agent-workspace/.claude/skills/commit.md"
    },
    {
      "name": "review",
      "description": "Review code changes",
      "command": "cat .agent-workspace/.claude/skills/review.md"
    },
    {
      "name": "pr",
      "description": "Create pull request with proper format",
      "command": "cat .agent-workspace/.claude/skills/pr.md"
    },
    {
      "name": "plan",
      "description": "Generate structured implementation or overview plans",
      "command": "cat .agent-workspace/.claude/skills/plan/SKILL.md"
    },
    {
      "name": "mcp-integration",
      "description": "Guide for integrating MCP servers into plugins",
      "command": "cat .agent-workspace/.claude/skills/mcp-integration/SKILL.md"
    }
  ]
}
```

## MCP Servers

Merge configurations from `.agent-workspace/.claude/mcp/` into your project settings.
