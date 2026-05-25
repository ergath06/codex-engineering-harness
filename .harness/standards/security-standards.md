# Security Standards

## Baseline

- Use secure defaults.
- Minimize privileges.
- Validate inputs at trust boundaries.
- Encode outputs for the destination context.
- Protect secrets and credentials.
- Avoid logging sensitive data.
- Keep dependencies current.
- Review authentication and authorization separately.

## Required For Sensitive Work

Use a threat model when the project includes:

- authentication or authorization
- payments
- personally identifiable information
- file uploads
- admin functionality
- public APIs
- AI-generated or user-generated content
- integrations with external systems

## Supply Chain

- Use dependency scanning.
- Generate an SBOM where appropriate.
- Pin or lock dependencies where practical.
- Review licenses for production use.
- Prefer trusted packages and official SDKs.
