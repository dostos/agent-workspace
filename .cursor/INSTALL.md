# Cursor Installation

## As Submodule

1. Add to your project:
   ```bash
   git submodule add <repo-url> .agent-workspace
   ```

2. Create symlink to cursorrules:
   ```bash
   ln -s .agent-workspace/.cursor/.cursorrules .cursorrules
   ```

Or include in your existing `.cursorrules`:
```
See .agent-workspace/AGENTS.md for coding conventions.
```
