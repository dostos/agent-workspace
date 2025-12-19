# Agent Workspace

Shared AI assistant configurations, skills, and MCP utilities for Claude Code, Cursor, and Codex.

## Installation

### Claude Code

```bash
git submodule add <repo-url> .agent-workspace
ln -s .agent-workspace/CLAUDE.md CLAUDE.md
```

See [.claude/INSTALL.md](.claude/INSTALL.md) for skills and MCP setup.

### Cursor

```bash
git submodule add <repo-url> .agent-workspace
ln -s .agent-workspace/.cursor/.cursorrules .cursorrules
```

### Codex

Tell Codex:
> Fetch and follow instructions from `<raw-url>/.codex/INSTALL.md`

## Structure

```
├── AGENTS.md                 # Shared instructions (source of truth)
├── CLAUDE.md                 # References @AGENTS.md
├── .claude/
│   ├── INSTALL.md
│   ├── skills/               # Slash commands
│   │   ├── commit.md         # /commit
│   │   ├── review.md         # /review
│   │   ├── pr.md             # /pr
│   │   ├── plan/             # /plan (with scripts)
│   │   └── mcp-integration/  # /mcp-integration (with refs)
│   └── mcp/
│       ├── README.md
│       └── servers/          # MCP server configs
├── .cursor/
│   ├── INSTALL.md
│   └── .cursorrules
└── .codex/
    └── INSTALL.md
```

## Skills

| Skill | Description |
|-------|-------------|
| `/commit` | Create module-prefixed conventional commit |
| `/review` | Review code changes |
| `/pr` | Create pull request |
| `/plan` | Generate structured implementation or overview plans |
| `/mcp-integration` | Guide for integrating MCP servers |

## Conventions

- Commits: `[module] type: message`
- Types: feat, fix, docs, style, refactor, test, chore
