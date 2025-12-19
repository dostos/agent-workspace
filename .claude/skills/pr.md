# /pr

Create a pull request with proper description.

## Instructions

1. Get branch info: `git branch --show-current`
2. Get commits: `git log main..HEAD --oneline`
3. Get full diff: `git diff main...HEAD`
4. Generate PR with:
   - Title: `[module] type: summary`
   - Description: what changed and why
   - Testing notes
5. Create PR: `gh pr create`

## Template

```markdown
## Summary
What this PR does

## Changes
- List of changes by module

## Testing
How to test these changes
```
