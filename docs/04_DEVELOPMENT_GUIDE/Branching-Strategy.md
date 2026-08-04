# Branching Strategy

## Purpose

The branching strategy helps contributors isolate work, reduce merge risk, and keep the main branch stable.

## Branch Types

| Branch Type | Naming Pattern | Purpose |
| --- | --- | --- |
| Main branch | `main` or repository default | Stable baseline for reviewed content. |
| Feature branch | `feature/<short-description>` | New documentation, standards, or functionality. |
| Fix branch | `fix/<short-description>` | Corrections to existing content or behavior. |
| Chore branch | `chore/<short-description>` | Maintenance, formatting, dependency, or tooling updates. |
| Release branch | `release/<version-or-date>` | Release preparation when formal releases are introduced. |

## Rules

- Keep branches focused and short-lived.
- Rebase or merge from the target branch when needed to resolve drift.
- Avoid mixing unrelated documentation, architecture, and tooling changes in one branch.
- Delete merged branches when no longer needed.

## Naming Examples

- `feature/enterprise-architecture-baseline`
- `fix/security-policy-reporting-channel`
- `chore/markdown-link-check`
