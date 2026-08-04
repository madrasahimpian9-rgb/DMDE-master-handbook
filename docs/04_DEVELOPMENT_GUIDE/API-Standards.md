# API Standards

## Purpose

API standards define how DMDE services expose capabilities through consistent, secure, versioned, and documented contracts.

## API Design Principles

- Use resource names that reflect business concepts and domain ownership.
- Version APIs when compatibility may be affected.
- Validate all request inputs and return consistent error responses.
- Apply authentication and authorization before returning protected data.
- Include pagination, filtering, sorting, and field-selection conventions where needed.
- Document request, response, status codes, errors, and examples before broad adoption.

## HTTP Guidance

| Concern | Standard |
| --- | --- |
| Success status | Use appropriate `2xx` responses for successful operations. |
| Client errors | Use `4xx` responses for validation, authorization, not found, and conflict cases. |
| Server errors | Use `5xx` responses for unexpected failures without leaking internals. |
| Pagination | Use consistent page, limit, cursor, or token conventions. |
| Idempotency | Use idempotency keys for retry-safe create or payment-like workflows. |
| Correlation | Accept or generate correlation IDs for traceability. |

## API Review Checklist

- [ ] Domain owner and contract owner are identified.
- [ ] Authentication and authorization behavior is documented.
- [ ] Error format and status codes are consistent.
- [ ] Backward compatibility and versioning impact are reviewed.
- [ ] Observability and audit events are defined where needed.
