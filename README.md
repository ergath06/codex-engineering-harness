# Codex Engineering Harness

Reusable engineering process assets for building software with Codex in a disciplined, human-reviewed workflow.

This repository defines a quality harness for requirements, architecture, implementation planning, controlled delivery, testing, security, accessibility, observability, release management, and post-release improvement.

## Purpose

The harness helps Codex and human reviewers collaborate through structured phases:

1. Harness setup and steering review.
2. Discovery and requirements.
3. Architecture and technical design.
4. Implementation planning.
5. Controlled implementation loops.
6. Final hardening and release readiness.
7. Post-release review.

The goal is not ceremony for its own sake. The goal is to make software work safer, clearer, faster, and easier to maintain.

## Repository Boundary

This repository is the reusable harness source. It should not be used as an application project repository.

For application work, create or use a separate project repository and import/copy the harness assets into that project. Modify this harness repository only when intentionally improving, fixing, or releasing the harness itself.

## Core Assets

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

AGENTS.md
CHANGELOG.md
RELEASE.md
```

## Template Tiers

The harness includes lightweight defaults for small work and fuller opt-in templates for larger or higher-risk projects.

Lightweight defaults:

- `.harness/templates/requirements.template.md`
- `.harness/templates/architecture.template.md`

Comprehensive templates:

- `.harness/templates/requirements-full.template.md`
- `.harness/templates/architecture-comprehensive.template.md`

Use the comprehensive templates when the project is ambiguous, regulated, security-sensitive, integration-heavy, multi-team, or expected to become a long-lived system.

## How To Use

For a new project, copy or import the `.harness/` directory and `AGENTS.md` into the project repository. Then create project-specific docs from the templates in `.harness/templates/`.

Recommended first project steps:

1. Read `.harness/HARNESS.md`.
2. Complete `.harness/templates/steering-assets-register.template.md`.
3. Create `docs/requirements.md` from the requirements template.
4. Pause for requirements approval.
5. Create `docs/architecture.md` and ADRs.
6. Pause for architecture approval.
7. Create an implementation plan.
8. Pause for implementation plan approval.
9. Implement in small reviewed increments.

## Version

Current baseline: `0.2.1`.

See [CHANGELOG.md](CHANGELOG.md) for notable changes.
