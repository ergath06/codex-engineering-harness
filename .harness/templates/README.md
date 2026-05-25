# Harness Templates

This directory contains reusable templates for Codex-guided software delivery.

## Template Tiers

Use the lightweight default templates for tiny changes, small projects, and low-risk features:

- `requirements.template.md`
- `architecture.template.md`
- `implementation-plan.template.md`
- `testing-strategy.template.md`

Use the fuller templates when the work is large, ambiguous, regulated, security-sensitive, multi-team, integration-heavy, or expected to become a long-lived system:

- `requirements-full.template.md`
- `architecture-comprehensive.template.md`

The fuller templates are opt-in steering assets. They should improve clarity, not create ceremony. If a section is not useful for the project, mark it `Not applicable` and explain why.

## Gate Alignment

Every project-facing template should preserve the harness gate loop protocol:

1. Approved to proceed.
2. Approved with non-blocking follow-ups.
3. Changes requested.
4. Loop back required.

Blocking feedback must be resolved before the next phase begins.
