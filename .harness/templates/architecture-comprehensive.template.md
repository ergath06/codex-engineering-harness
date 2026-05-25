# [Project Name] - Comprehensive Software Architecture Document

> Template purpose: This is a comprehensive architecture template for larger, higher-risk, integration-heavy, or long-lived systems.
>
> Authoring guidance: Use the sections that improve clarity. If a section is not useful for the project, mark it `Not applicable` and explain why. Diagrams are required only when they clarify decisions, risks, interfaces, or behavior.

## Document Control

- Project Name: `[Insert project name]`
- Version: `[Insert version]`
- Date: `[YYYY-MM-DD]`
- Status: `[Draft / In review / Approved / Superseded]`
- Owner: `[Architecture owner]`
- Reviewers: `[Human reviewers]`
- Related Requirements: `[Requirements document/version]`
- Selected Steering Assets: `[Templates, standards, reference architectures]`

## 1. Document Overview

Purpose: Define the identity of the system and orient readers before technical detail.

### 1.1 Purpose

`[Describe the purpose of this architecture document, such as guiding development, stakeholder communication, compliance, or operational readiness.]`

### 1.2 System Scope

Inside the system:

- `[In-scope boundary]`

Outside the system:

- `[Out-of-scope boundary]`

### 1.3 Stakeholders

| Stakeholder | Role | Concerns |
| --- | --- | --- |
| `[Stakeholder]` | `[Role]` | `[Maintainability, security, performance, operations, compliance, etc.]` |

## 2. Architecture Goals And Constraints

Purpose: Capture the requirements, quality attributes, constraints, and steering assets that drive design decisions.

### 2.1 Quality Attributes

| Attribute | Target | Source Requirement | Validation |
| --- | --- | --- | --- |
| Performance | `[Latency, throughput, response time]` | `[NFR ID]` | `[Test or review method]` |
| Scalability | `[Growth target]` | `[NFR ID]` | `[Test or review method]` |
| Security | `[Control target]` | `[NFR ID]` | `[Test or review method]` |
| Privacy | `[Data handling target]` | `[NFR ID]` | `[Test or review method]` |
| Accessibility | `[Target, e.g., WCAG 2.2 AA]` | `[NFR ID]` | `[Test or review method]` |
| Availability / Reliability | `[Uptime, RTO, RPO]` | `[NFR ID]` | `[Test or review method]` |
| Observability | `[Logs, metrics, traces, alerts]` | `[NFR ID]` | `[Test or review method]` |

### 2.2 Constraints

Technical constraints:

- `[Mandated technologies, legacy systems, hardware limits, platform constraints]`

Organizational constraints:

- `[Budget, timeline, team skills, compliance obligations, support model]`

### 2.3 Steering Asset Alignment

| Asset | Applies How | Deviations | Rationale |
| --- | --- | --- | --- |
| `[Template / standard / reference architecture]` | `[How it guides this design]` | `[Deviation, if any]` | `[Why]` |

## 3. System Context And Scope

Purpose: Show how the system fits into the broader ecosystem.

### 3.1 System Context Diagram

Use C4 Level 1, Mermaid, or text.

```text
[External User / System]
    |
[System Under Design]
    |
[External Dependency]
```

### 3.2 Business Context

`[Describe the business domain and how the system supports business processes.]`

### 3.3 External Actors And Systems

| Actor / System | Relationship | Data Exchanged | Criticality |
| --- | --- | --- | --- |
| `[Actor or external system]` | `[How it interacts]` | `[Data or events]` | `[Critical / Important / Optional]` |

## 4. Solution Strategy And Architecture Decisions

Purpose: Explain the high-level design approach and justify major decisions.

### 4.1 Architectural Strategy

Chosen architecture style:

- `[Monolith / modular monolith / microservices / event-driven / serverless / layered / clean architecture / other]`

Rationale:

`[Explain why this style fits the approved requirements, constraints, and risk profile.]`

### 4.2 Technology Stack

- Frontend: `[Technology]`
- Backend: `[Technology]`
- Database: `[Technology]`
- Infrastructure: `[Technology]`
- Observability: `[Technology]`
- CI/CD: `[Technology]`

### 4.3 Architecture Decision Records

For each major decision, create or link an ADR in `docs/adr/`.

| ADR | Decision | Status | Related Requirements |
| --- | --- | --- | --- |
| ADR-0001 | `[Decision]` | `[Proposed / Accepted / Superseded]` | `[Requirement IDs]` |

## 5. Functional View

Purpose: Describe system behavior from the user's perspective.

### 5.1 Critical Use Cases

For each critical use case:

- Primary Actor And Goal:
- Preconditions:
- Main Success Scenario:
- Alternate / Exception Flows:
- Postconditions:
- Related Requirements:

### 5.2 Use Case To Component Mapping

| Use Case | Components Involved | Related Requirements | Notes |
| --- | --- | --- | --- |
| `[Use case]` | `[Components]` | `[FR IDs]` | `[Notes]` |

## 6. Structural View

Purpose: Define the static structure of the system.

### 6.1 Domain Model

Conceptual business entities:

| Entity | Responsibility / Meaning | Key Relationships |
| --- | --- | --- |
| `[Entity]` | `[Meaning]` | `[Relationships]` |

### 6.2 Container View

Use C4 Level 2, Mermaid, or text.

| Container | Responsibility | Technology | Dependencies |
| --- | --- | --- | --- |
| `[Web app / API / database / worker]` | `[Responsibility]` | `[Technology]` | `[Dependencies]` |

### 6.3 Component View

Use component diagrams only where they improve clarity.

| Component | Responsibility | Interfaces | Dependencies |
| --- | --- | --- | --- |
| `[Component]` | `[Responsibility]` | `[Interfaces]` | `[Dependencies]` |

### 6.4 Class Or Object Model

Use UML or equivalent diagrams only for complex domain models or tricky object interactions.

`[Diagram or explanation goes here, or mark Not applicable.]`

## 7. Behavioral View

Purpose: Describe how the system behaves over time.

### 7.1 System Sequence Flows

| Flow | Trigger | Main Steps | Failure Modes |
| --- | --- | --- | --- |
| `[Flow]` | `[Trigger]` | `[Steps]` | `[Failure modes]` |

### 7.2 Detailed Sequence Diagrams

Use detailed diagrams for integration-heavy or risky flows.

`[Diagram or explanation goes here, or mark Not applicable.]`

### 7.3 State Models

Use state machines for entities with meaningful lifecycles.

| Entity | States | Transitions | Invalid Transitions |
| --- | --- | --- | --- |
| `[Entity]` | `[States]` | `[Transitions]` | `[Invalid transitions]` |

### 7.4 Activity Or Workflow Diagrams

`[Diagram or explanation goes here, or mark Not applicable.]`

## 8. Data View

Purpose: Explain how data is structured, stored, protected, and moved.

### 8.1 Logical Data Model

| Entity | Key Attributes | Relationships | Related Requirements |
| --- | --- | --- | --- |
| `[Entity]` | `[Attributes]` | `[Relationships]` | `[Requirement IDs]` |

### 8.2 Physical Data Model

| Store | Structure | Keys / Indexes | Notes |
| --- | --- | --- | --- |
| `[Database / table / collection / file store]` | `[Structure]` | `[Keys or indexes]` | `[Notes]` |

### 8.3 Data Flow

`[Describe data movement, transformations, and trust boundaries.]`

### 8.4 Data Dictionary

| Data Element | Format | Meaning | Validation |
| --- | --- | --- | --- |
| `[Element]` | `[Format]` | `[Meaning]` | `[Validation]` |

### 8.5 Data Classification And Retention

| Data Type | Classification | Storage | Transmission | Retention | Deletion |
| --- | --- | --- | --- | --- | --- |
| `[Data type]` | `[Public / Internal / Confidential / Restricted]` | `[Storage]` | `[Transmission]` | `[Retention]` | `[Deletion approach]` |

## 9. Interface And User Experience View

Purpose: Connect user experience, system behavior, and interface contracts.

### 9.1 UI Architecture

- Screen flows:
- Navigation:
- State management:
- Accessibility model:
- Error presentation:

### 9.2 UI-To-Logic Mapping

| UI Action | System Behavior | API / Component | Failure Handling |
| --- | --- | --- | --- |
| `[Action]` | `[Behavior]` | `[API or component]` | `[Failure handling]` |

### 9.3 API Specifications

| Interface | Style | Consumers | Contract Location |
| --- | --- | --- | --- |
| `[API]` | `[REST / GraphQL / gRPC / events / other]` | `[Consumers]` | `[OpenAPI / schema / docs path]` |

### 9.4 Accessibility Strategy

Define:

- target standard
- semantic structure
- keyboard interaction
- focus management
- screen reader behavior
- color and contrast approach
- validation approach

## 10. Physical And Deployment View

Purpose: Map logical components to infrastructure.

### 10.1 Deployment Topology

`[Diagram or text showing runtime deployment topology.]`

### 10.2 Network And Topology

- Load balancers:
- Network boundaries:
- Firewall rules:
- Private/public endpoints:
- External connectivity:

### 10.3 Environments

| Environment | Purpose | Data | Deployment Method | Differences |
| --- | --- | --- | --- | --- |
| Development | `[Purpose]` | `[Data]` | `[Method]` | `[Differences]` |
| Staging | `[Purpose]` | `[Data]` | `[Method]` | `[Differences]` |
| Production | `[Purpose]` | `[Data]` | `[Method]` | `[Differences]` |

### 10.4 Rollback And Recovery

- Rollback trigger:
- Rollback method:
- Data migration rollback:
- Recovery time objective:
- Recovery point objective:
- Smoke tests after rollback:

## 11. Implementation View

Purpose: Provide developers with code organization guidance.

### 11.1 Source Code Structure

```text
[Proposed repo structure]
```

### 11.2 Layering And Boundaries

| Layer / Boundary | Responsibility | Allowed Dependencies | Prohibited Dependencies |
| --- | --- | --- | --- |
| `[Layer]` | `[Responsibility]` | `[Allowed]` | `[Prohibited]` |

### 11.3 Build And Configuration

- Build system:
- Dependency management:
- Configuration handling:
- Secret management:
- Local development setup:

### 11.4 Dependency Strategy

| Dependency | Purpose | Risk | Approval / Governance |
| --- | --- | --- | --- |
| `[Dependency]` | `[Purpose]` | `[Risk]` | `[Approval or policy]` |

## 12. Quality Assurance And Testing Strategy

Purpose: Explain how the architecture will be validated.

### 12.1 Test Strategy

- Unit testing:
- Integration testing:
- End-to-end testing:
- Accessibility testing:
- Security testing:
- Performance testing:
- Acceptance testing:

### 12.2 Traceability Matrix

| Requirement | Component | Test Evidence | Status |
| --- | --- | --- | --- |
| `[Requirement ID]` | `[Component]` | `[Test or review evidence]` | `[Status]` |

### 12.3 Quality Attribute Scenarios

| Attribute | Source | Stimulus | Environment | Response | Response Measure |
| --- | --- | --- | --- | --- | --- |
| `[Attribute]` | `[Source]` | `[Stimulus]` | `[Environment]` | `[Response]` | `[Measure]` |

## 13. Cross-Cutting Concerns

Purpose: Capture concerns that span the entire system.

### 13.1 Security Architecture

- Authentication:
- Authorization:
- Input validation:
- Output encoding:
- Encryption at rest:
- Encryption in transit:
- Audit logging:
- Secrets handling:
- Abuse cases:
- Threat model location:

### 13.2 Privacy Architecture

- Personal data categories:
- Consent or legal basis:
- Minimization:
- Retention:
- Deletion:
- Data subject access:
- Logging restrictions:

### 13.3 Observability

- Structured logs:
- Metrics:
- Traces:
- Correlation IDs:
- Dashboards:
- Alerts:
- Runbooks:

### 13.4 Error Handling

- User-facing errors:
- API errors:
- Retry strategy:
- Timeout strategy:
- Circuit breaker / bulkhead strategy where applicable:
- Dead-letter or recovery handling:

## 14. Risks And Roadmap

Purpose: Track uncertainties and future evolution.

### 14.1 Risk Log

| ID | Risk | Likelihood | Impact | Mitigation |
| --- | --- | --- | --- | --- |
| AR-001 | `[Risk]` | `[Low / Medium / High]` | `[Low / Medium / High]` | `[Mitigation]` |

### 14.2 Technical Debt

| Debt Item | Reason Accepted | Risk | Remediation Target |
| --- | --- | --- | --- |
| `[Debt item]` | `[Reason]` | `[Risk]` | `[Target]` |

### 14.3 Roadmap

| Future Item | Trigger | Notes |
| --- | --- | --- |
| `[Enhancement / scaling step]` | `[When it matters]` | `[Notes]` |

## 15. Appendices

### 15.1 Glossary

| Term | Definition |
| --- | --- |
| `[Term]` | `[Definition]` |

### 15.2 References

| Reference | Location | Notes |
| --- | --- | --- |
| `[Standard / regulatory document / design guideline]` | `[Link or path]` | `[Notes]` |

### 15.3 Diagram Inventory

| Diagram | Required | Location | Notes |
| --- | --- | --- | --- |
| System context | `[Yes / No]` | `[Path]` | `[Notes]` |
| Container view | `[Yes / No]` | `[Path]` | `[Notes]` |
| Component view | `[Yes / No]` | `[Path]` | `[Notes]` |
| Sequence flow | `[Yes / No]` | `[Path]` | `[Notes]` |
| State model | `[Yes / No]` | `[Path]` | `[Notes]` |

## 16. AI Authoring Guidance

When completing this template, Codex should:

1. Align every architecture decision to approved requirements.
2. Keep architecture proportional to project scale and risk.
3. Use diagrams only when they clarify a decision, behavior, dependency, or risk.
4. Record major decisions as ADRs.
5. Surface tradeoffs and residual risks explicitly.
6. Include security, privacy, accessibility, observability, rollback, and dependency strategy.
7. Identify where requirements need refinement before design can be approved.
8. Avoid copying reference architecture code or structure blindly.

## Gate Decision

- [ ] Approved to proceed
- [ ] Approved with non-blocking follow-ups
- [ ] Changes requested
- [ ] Loop back required

Decision notes:
