# Harness Architecture

The harness repository is organized as reusable process assets plus project-facing documentation.

## Structure

```text
.harness/
  HARNESS.md
  templates/
  standards/
  checklists/
  reference-architectures/

docs/
  adr/
  requirements.md
  architecture.md
  security.md
  accessibility.md
  testing.md
  operations.md

examples/
  project-structures/
```

## Design Choices

- `.harness/` contains reusable assets intended to be copied or imported into application repositories.
- `docs/` contains documentation for this harness repository.
- `AGENTS.md` gives Codex explicit operating instructions.
- Reference architectures are isolated so framework-specific examples do not pollute the core process.

## Extension Points

- Add templates under `.harness/templates/`.
- Add standards under `.harness/standards/`.
- Add checklists under `.harness/checklists/`.
- Add validated examples under `.harness/reference-architectures/<name>/sample-app/`.
