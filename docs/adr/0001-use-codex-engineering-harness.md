# ADR-0001: Use A Codex Engineering Harness

Date: 2026-05-24
Status: accepted

## Context

Codex-assisted development benefits from durable, explicit process assets that survive beyond a single chat or workspace. The process should support requirements, architecture, planning, implementation, testing, review, release, and continuous improvement.

## Decision

Create a dedicated `codex-engineering-harness` repository that contains reusable templates, standards, checklists, reference architecture placeholders, and Codex operating instructions.

## Consequences

- Projects can import a consistent operating model.
- Human review gates become explicit.
- Reference assets can evolve over time.
- Project-specific adaptations remain possible.

## Alternatives Considered

- Rely only on chat instructions. Rejected because instructions are less durable and less reviewable.
- Embed the harness only in each project. Rejected because reusable improvements would be harder to share.
- Build a tool-agnostic harness first. Deferred so this repository can be tuned for Codex workflows.
