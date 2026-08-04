# Logging Standards

## Purpose

Logging standards help teams diagnose issues, support audits, monitor operations, and troubleshoot cross-domain workflows without exposing sensitive data.

## Logging Principles

- Use structured logs instead of unstructured text where possible.
- Include correlation IDs, request IDs, user or service context, and domain identifiers when appropriate.
- Never log passwords, tokens, secrets, private keys, or unnecessary personal data.
- Use consistent severity levels and actionable messages.
- Ensure logs support incident response and operational dashboards.

## Severity Levels

| Level | Usage |
| --- | --- |
| Debug | Detailed diagnostic information for development or controlled troubleshooting. |
| Info | Normal workflow milestones and operational state changes. |
| Warn | Recoverable issues, degraded behavior, retries, or suspicious input. |
| Error | Failed operations requiring investigation or user-visible failure. |
| Critical | System-level failures, security incidents, or severe operational impact. |

## Required Context

- Timestamp.
- Severity.
- Service or component name.
- Correlation or trace identifier.
- Operation or workflow name.
- Safe actor or organization context when authorized and useful.
