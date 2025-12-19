# /commit

Create a module-prefixed conventional commit.

## Instructions

1. Run `git status` and `git diff --cached` to see staged changes
2. Identify the module from the file paths (e.g., `src/auth/` → `auth`)
3. Determine commit type:
   - `feat`: new feature
   - `fix`: bug fix
   - `docs`: documentation
   - `style`: formatting
   - `refactor`: restructuring
   - `test`: tests
   - `chore`: maintenance
4. Format: `[module] type: concise description`
5. Execute the commit

## Examples

- `[auth] feat: add JWT refresh token support`
- `[api] fix: handle timeout errors gracefully`
- `[cli] refactor: extract argument parsing`
