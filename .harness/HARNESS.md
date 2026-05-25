# Engineering Harness

Version: `0.1.0`

## Purpose

This harness governs how we design, build, validate, document, and release software with Codex. It is designed to produce maintainable, secure, accessible, observable, production-quality applications through controlled iterative development with human-in-the-loop checkpoints.

## Core Principles

- Requirements drive architecture.
- Architecture drives implementation.
- Implementation remains traceable to requirements and architecture.
- Tests validate real behavior, edge cases, and failure modes.
- Security, accessibility, observability, maintainability, and documentation are first-class requirements.
- Human review gates are mandatory before major phase transitions.
- Every gate supports revision, re-review, and looping back.
- Automation improves quality and speed without replacing judgment.
- Major decisions are explainable, documented, and traceable.
- Process weight scales with project size, complexity, and risk.
- Reference examples guide implementation but do not override approved requirements or architecture.

## Project Scale Classification

Classify the work before choosing artifact depth:

- Tiny change: small isolated fix or update.
- Small project or feature: limited scope, low risk, few integrations.
- Product feature: user-facing or shared behavior.
- Enterprise or high-risk system: regulated, security-sensitive, revenue-critical, multi-team, data-sensitive, or operationally complex.

## Steering Assets And Templates

Projects may include steering material that guides planning and implementation:

- document templates
- architecture templates
- reference architectures
- example applications
- framework-specific starter solutions
- coding standards
- API standards
- UI/component examples
- testing examples
- CI/CD examples
- deployment templates
- security checklists
- accessibility checklists
- observability standards
- ADR templates
- release checklist templates

Before implementation begins, relevant steering assets must be identified and reviewed. If a target architecture, platform, or framework is selected, corresponding reference assets should guide planning and implementation unless explicitly overridden.

Reference assets are guidance, not automatic source of truth. If a reference example conflicts with approved requirements, security needs, accessibility needs, maintainability goals, or architecture decisions, the conflict must be documented and resolved intentionally.

## Universal Gate Loop Protocol

At every human review checkpoint, the reviewer can choose:

1. Approved to proceed.
2. Approved with non-blocking follow-ups.
3. Changes requested.
4. Loop back required.

No phase is complete until blocking feedback is resolved and the revised artifacts are approved.

## Phase 0 - Harness Setup And Steering Review

Before project-specific discovery:

1. Confirm project scale classification.
2. Identify relevant templates.
3. Identify relevant reference architectures.
4. Identify coding, testing, security, accessibility, and observability standards.
5. Identify reusable examples or starter solutions.
6. Record selected steering assets.
7. Record intentionally skipped steering assets.
8. Identify gaps in the harness itself.

Outputs:

- steering assets register
- project scale classification
- initial process tailoring notes

Gate: steering review.

## Phase 1 - Discovery And Requirements

Capture:

- business goals
- users and use cases
- functional requirements
- non-functional requirements
- assumptions and unknowns
- constraints and risks
- acceptance criteria
- out-of-scope items
- integration dependencies
- traceable requirements document

Outputs:

- requirements document
- assumptions log
- risk register
- acceptance criteria
- requirements traceability matrix

Gate: requirements review.

## Phase 2 - Architecture And Technical Design

Create:

- system architecture
- component/service breakdown
- data flow description or diagram
- API/interface definitions
- data models
- state management strategy
- error handling strategy
- authentication and authorization strategy
- security model
- accessibility strategy
- observability/logging strategy
- deployment/environment strategy
- testing strategy
- dependency strategy
- rollback/recovery strategy
- architecture decision records for major choices

Evaluate:

- tradeoffs
- technical debt risks
- framework and dependency choices
- alignment with selected steering assets

Outputs:

- architecture document
- ADRs
- data model notes
- API/interface contracts
- threat model where applicable

Gate: architecture review.

## Phase 3 - Implementation Planning

Create:

- iterative roadmap
- milestone breakdown
- task hierarchy
- dependency sequencing
- risk-prioritized work order
- test coverage plan
- Definition of Ready
- Definition of Done
- validation checkpoints
- CI/CD recommendations
- branching/version control approach
- documentation update plan

Each iteration must:

- be small enough to review safely
- produce a working validated increment
- include tests and documentation updates

Gate: implementation plan review.

## Phase 4 - Controlled Implementation Loop

For each iteration:

1. Pre-implementation review.
2. Implementation.
3. Testing.
4. Validation and review.
5. Iteration if issues exist.

Implementation must be clean, modular, maintainable, secure, accessible where user-facing, observable where operationally relevant, and documented where needed.

Tests must validate meaningful behavior, include edge cases, verify failure modes, and avoid artificial passing.

Gate: milestone review after each major or high-risk increment.

## Phase 5 - Final Hardening And Readiness Review

Perform:

- full requirements traceability review
- architecture consistency review
- steering asset alignment review
- security review
- accessibility review
- performance review
- dependency audit
- documentation audit
- observability review
- deployment readiness review
- rollback verification
- test suite quality review

Generate:

- known limitations
- technical debt summary
- future improvement recommendations
- operational considerations
- maintenance guidance
- release notes

Gate: final release approval.

## Phase 6 - Post-Release Review

After release:

- review production behavior
- review incidents or defects
- compare outcomes against requirements
- capture lessons learned
- update documentation
- update steering assets where reusable improvements were discovered
- update the harness if needed

Outputs:

- post-release review notes
- follow-up backlog
- harness improvement notes

## Quality Gates

Recommended automated gates:

- formatting
- linting
- type checking
- unit tests
- integration tests
- end-to-end tests where applicable
- accessibility checks
- dependency vulnerability scan
- secret scan
- static security analysis
- license check
- SBOM generation where appropriate
- build verification
- deployment smoke test
- coverage reporting
