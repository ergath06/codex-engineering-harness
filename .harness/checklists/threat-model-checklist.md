# Threat Model Checklist

Use this checklist when the project handles sensitive data, authentication, authorization, external integrations, file uploads, public APIs, payments, or administrative actions.

## Assets

- [ ] Sensitive data identified.
- [ ] Critical operations identified.
- [ ] External dependencies identified.

## Actors

- [ ] Legitimate users identified.
- [ ] Privileged users identified.
- [ ] Anonymous or external actors identified.
- [ ] Abuse cases identified.

## Boundaries

- [ ] Trust boundaries identified.
- [ ] Input boundaries identified.
- [ ] External service boundaries identified.

## Controls

- [ ] Authentication reviewed.
- [ ] Authorization reviewed.
- [ ] Input validation reviewed.
- [ ] Output encoding reviewed.
- [ ] Secrets handling reviewed.
- [ ] Logging reviewed for sensitive data.
- [ ] Dependency risks reviewed.

## Validation

- [ ] Security tests identified.
- [ ] Manual review items identified.
- [ ] Residual risks documented.
