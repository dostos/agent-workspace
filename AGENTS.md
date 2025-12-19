# Agent Instructions

Shared instructions for all AI coding assistants.

## General Rules

- Write clean, maintainable code
- Follow existing project conventions
- Prefer simple solutions over complex ones
- Add tests for new functionality
- Use meaningful variable and function names

## Code Style

- Use consistent formatting
- Keep functions small and focused
- Avoid deep nesting
- Handle errors appropriately

## Git Conventions

- Use module-prefixed conventional commits: `[module-name] type: message`
  - Examples:
    - `[auth] feat: add OAuth2 support`
    - `[api] fix: handle null response`
    - `[docs] chore: update README`
  - Types: feat, fix, docs, style, refactor, test, chore
- Keep commits atomic and focused
- Write descriptive commit messages

## Security

- Never commit secrets or credentials
- Validate user inputs
- Use parameterized queries for databases
