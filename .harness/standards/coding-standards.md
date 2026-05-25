# Coding Standards

## Principles

- Prefer clarity over cleverness.
- Keep modules cohesive and responsibilities explicit.
- Follow established project conventions before introducing new patterns.
- Avoid unnecessary abstractions.
- Keep side effects visible.
- Treat warnings as meaningful signals.
- Document decisions, not obvious mechanics.

## Maintainability

- Use descriptive names.
- Keep functions small enough to reason about.
- Keep dependency direction intentional.
- Prefer pure functions for business logic where practical.
- Isolate framework and infrastructure details from domain logic when the project size justifies it.

## Error Handling

- Handle expected failures intentionally.
- Do not swallow exceptions silently.
- Preserve diagnostic context without leaking sensitive data.
- Return user-safe error messages at boundaries.

## Documentation

- Update docs with behavior changes.
- Use ADRs for meaningful architecture decisions.
- Keep comments rare and useful.
