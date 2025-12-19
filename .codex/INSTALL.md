# Codex Installation

## Setup

1. Add this repository as a submodule:
   ```bash
   git submodule add <repo-url> .agent-workspace
   ```

2. The AGENTS.md in the root contains shared instructions.

## Usage

Follow the conventions in `AGENTS.md` for:
- Code style
- Git commits: `[module-name] type: message`
- Security practices

## Skills

Available skills can be invoked by asking Codex to follow instructions from:
- `.agent-workspace/.codex/skills/commit.md`
- `.agent-workspace/.codex/skills/review.md`
