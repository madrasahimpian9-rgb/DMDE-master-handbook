# Jendela Nilai Domain Architecture

## Domain Purpose

Provide a focused grade-window experience for reviewing, validating, publishing, and communicating learner scores and progress.

## Business Outcomes

- Provide a clear system of record for the domain's core responsibilities.
- Standardize workflows, rules, and ownership expectations for related capabilities.
- Support secure, auditable, and reportable operations across stakeholder groups.
- Enable integration with other DMDE domains through explicit contracts and events.

## Core Concepts

| Concept Area | Description |
| --- | --- |
| Core entities | Grade Window, Score View, Validation Status, Publication State. |
| Primary workflows | score review, validation, publication, grade visibility, correction request. |
| Ownership | Define the product owner, domain owner, data owner, and operational owner for this domain. |
| Data quality | Document required fields, validation rules, lifecycle states, and reconciliation expectations. |
| Auditability | Identify sensitive actions that must be logged with actor, action, target, timestamp, and context. |

## Integration Expectations

- Publish APIs or events only with documented contracts and owners.
- Identify upstream data sources and downstream consumers.
- Define failure handling, retry expectations, and reconciliation steps for cross-domain workflows.
- Link integration decisions to enterprise architecture records when they affect shared standards.

## Security and Privacy Considerations

- Apply least-privilege access based on role, permission, and organization context.
- Classify sensitive records and avoid exposing unauthorized personal, academic, or operational data.
- Preserve audit evidence for approvals, status changes, publication actions, and administrative overrides.

## Reporting Considerations

- Define metrics, dimensions, filters, and source-of-truth data for reporting needs.
- Document calculation rules and transformation logic before reports depend on them.
- Identify data freshness, retention, and export requirements.

## Open Questions

- Which stakeholders approve domain-specific business rules?
- Which cross-domain dependencies must be resolved before implementation?
- What non-functional requirements are critical for this domain's release readiness?
