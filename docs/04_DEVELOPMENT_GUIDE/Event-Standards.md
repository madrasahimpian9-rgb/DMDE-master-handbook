# Event Standards

## Purpose

Event standards ensure DMDE asynchronous communication is meaningful, reliable, observable, and safe for cross-domain consumption.

## Event Design Principles

- Publish events for meaningful business facts, not internal implementation details.
- Name events with past-tense business language, such as `StudentEnrolled` or `AssessmentPublished`.
- Include producer, schema version, timestamp, correlation ID, and business identifier.
- Avoid sensitive payloads unless explicitly approved and protected.
- Document expected ordering, retry, idempotency, and dead-letter behavior.

## Event Metadata

| Field | Purpose |
| --- | --- |
| `eventId` | Unique identifier for deduplication and traceability. |
| `eventType` | Business event name. |
| `eventVersion` | Schema version for compatibility management. |
| `occurredAt` | Time the business fact occurred. |
| `producer` | Domain or service that emitted the event. |
| `correlationId` | Trace identifier across workflows. |

## Review Checklist

- [ ] Event represents a domain fact.
- [ ] Schema and version are documented.
- [ ] Consumers and failure handling are known.
- [ ] Sensitive data exposure is reviewed.
- [ ] Monitoring and replay expectations are defined.
