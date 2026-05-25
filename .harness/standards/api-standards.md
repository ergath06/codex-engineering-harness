# API Standards

## Design

- APIs must map to clear use cases.
- Request and response contracts must be documented.
- Validation rules must be explicit.
- Error responses must be consistent.
- Breaking changes must be versioned or coordinated.

## Security

- Authenticate every protected operation.
- Authorize by resource and action, not only by role name.
- Validate all inputs at trust boundaries.
- Avoid leaking sensitive data in responses or errors.

## Reliability

- Define idempotency expectations for write operations.
- Use timeouts and retries intentionally.
- Document rate limits where applicable.
- Include correlation IDs for diagnostics.

## Observability

- Log request outcomes without logging secrets.
- Capture latency, error rate, and saturation metrics.
- Trace calls across service boundaries where applicable.
