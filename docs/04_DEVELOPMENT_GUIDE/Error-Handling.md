# Error Handling

## Purpose

Error handling standards ensure failures are predictable, secure, actionable, observable, and consistent across DMDE capabilities.

## Error Principles

- Fail safely and preserve data integrity.
- Return user-facing messages that are helpful but do not expose sensitive internals.
- Capture diagnostic details in logs with appropriate access controls.
- Use consistent error codes and categories across APIs and workflows.
- Distinguish validation, authentication, authorization, not found, conflict, dependency, and unexpected errors.

## Error Categories

| Category | Description | Typical Response |
| --- | --- | --- |
| Validation | Input does not satisfy required format or rules. | Explain field-level issues. |
| Authentication | User or service is not authenticated. | Ask for valid authentication. |
| Authorization | Authenticated actor lacks permission. | Deny without exposing protected details. |
| Not found | Requested resource does not exist or is not visible to actor. | Return safe not-found response. |
| Conflict | Request conflicts with current state or business rule. | Explain conflict and possible next action. |
| Dependency | External service or integration failed. | Retry when safe or surface temporary failure. |
| Unexpected | Unhandled system error. | Return generic response and log diagnostics. |

## Checklist

- [ ] Error response format is consistent.
- [ ] Sensitive details are excluded from user-facing responses.
- [ ] Logs contain enough diagnostic context.
- [ ] Retry and compensation behavior are documented where applicable.
