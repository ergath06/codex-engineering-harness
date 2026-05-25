# Observability Standards

## Goals

Systems should explain what happened, why it happened, who or what was affected, and what action is needed.

## Logs

- Use structured logs.
- Include correlation or request IDs.
- Avoid secrets and sensitive personal data.
- Log important state transitions and failures.

## Metrics

- Track request count, latency, errors, and saturation where applicable.
- Track domain-specific success and failure signals.
- Define service-level indicators for critical systems.

## Traces

- Trace cross-service calls where applicable.
- Propagate context across boundaries.
- Capture relevant spans without excessive noise.

## Alerts

- Alert on user impact and actionable failure modes.
- Avoid noisy alerts.
- Link alerts to runbooks where practical.
