# Coding Standards

## Purpose

Coding standards keep DMDE implementations readable, maintainable, secure, and consistent across teams and domains.

## General Standards

- Prefer clear, descriptive names for modules, functions, variables, files, APIs, and events.
- Keep functions and components focused on one responsibility.
- Separate domain logic from transport, persistence, presentation, and infrastructure concerns.
- Validate inputs at system boundaries and enforce business rules in the appropriate domain layer.
- Avoid committing secrets, generated files, local configuration, or sensitive sample data.
- Update related documentation when implementation behavior changes.

## Code Quality Expectations

| Area | Expectation |
| --- | --- |
| Readability | Code should be understandable without relying on hidden context or excessive comments. |
| Modularity | Domain boundaries and shared-kernel responsibilities should remain clear. |
| Error handling | Errors should be explicit, actionable, and safe to expose where appropriate. |
| Security | Authorization, validation, and data protection must be considered during design and review. |
| Observability | Important workflows should provide structured logs, metrics, and trace context. |
| Testing | Critical behavior should have automated tests or documented manual validation steps. |

## Review Checklist

- [ ] Code follows naming and structure conventions.
- [ ] Domain logic is not duplicated across unrelated modules.
- [ ] Inputs, permissions, and error cases are handled.
- [ ] Tests or validation notes cover meaningful behavior.
- [ ] Documentation and changelog updates are included when needed.
