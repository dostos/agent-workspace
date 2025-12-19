# /review

Review code changes for issues and improvements.

## Instructions

1. Get changes: `git diff` (unstaged) or `git diff --cached` (staged)
2. Analyze for:
   - Logic errors and bugs
   - Security vulnerabilities
   - Performance issues
   - Missing error handling
   - Code style violations
3. Provide feedback with file:line references
4. Suggest specific fixes

## Output Format

```
## Summary
Brief overview of changes

## Issues
- [severity] file:line - description

## Suggestions
- file:line - improvement idea
```
