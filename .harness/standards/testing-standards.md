# Testing Standards

## Principles

- Tests must validate meaningful behavior.
- Tests must cover important edge cases and failure modes.
- Tests should fail for real regressions.
- Avoid tests that only assert implementation trivia.
- Avoid artificial passing through excessive mocking.

## Test Types

- Unit tests for focused logic.
- Integration tests for module and infrastructure boundaries.
- End-to-end tests for critical user journeys.
- Accessibility tests for user-facing flows.
- Security tests for trust boundaries and abuse cases.
- Performance tests for explicit performance requirements.

## Quality

- Test names should explain behavior.
- Test data should be intentional and maintainable.
- Flaky tests must be fixed or quarantined with a tracked follow-up.
- Coverage metrics are signals, not the goal.
