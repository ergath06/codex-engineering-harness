# Codex Operating Instructions

This repository contains the Codex Engineering Harness. When working in this repository or in a project that imports these assets, Codex must follow the harness unless the human reviewer explicitly approves a different process.

## Repository Boundary Rule

The `codex-engineering-harness` repository is the reusable source for process assets. Do not modify this repository when building an application unless the human explicitly asks to improve, fix, or release the harness itself.

For application work, create or use a separate project repository and import/copy the harness assets into that project. Project-specific requirements, architecture, implementation plans, ADRs, tests, and application code belong in the application repository, not in the harness source repository.

If a project reveals a reusable process improvement, record it as a harness follow-up. Apply it to this repository only after the human explicitly approves a harness change.

## Required Behavior

Before writing or modifying application code:

1. Read `.harness/HARNESS.md`.
2. Identify relevant templates, standards, checklists, and reference architectures.
3. Establish project scale: tiny change, small project, product feature, or enterprise/high-risk system.
4. Create or update the required planning artifacts.
5. Pause at the appropriate human review gate.

Use lightweight templates by default. Use `requirements-full.template.md` and `architecture-comprehensive.template.md` when the project is large, ambiguous, regulated, security-sensitive, integration-heavy, multi-team, or expected to become a long-lived system.

## Human Gates

Every gate supports four outcomes:

1. Approved to proceed.
2. Approved with non-blocking follow-ups.
3. Changes requested.
4. Loop back required.

Blocking feedback must be resolved before moving to the next phase.

## Implementation Rules

Codex must:

- keep requirements, architecture, tests, and documentation aligned
- use reference architectures as guidance, not blind copy sources
- preserve project-specific decisions in ADRs
- write meaningful tests that validate behavior and failure modes
- surface security, accessibility, observability, and maintainability risks early
- avoid speculative architecture and unnecessary abstractions
- update documentation alongside implementation

## Review Stance

When reviewing code or plans, prioritize:

1. correctness and requirement alignment
2. security and privacy
3. accessibility
4. reliability and operational readiness
5. test quality
6. maintainability
7. documentation and traceability
