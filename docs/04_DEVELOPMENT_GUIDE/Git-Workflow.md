# Git Workflow

## Purpose

The Git workflow defines how contributors prepare, review, and merge changes to the DMDE Master Handbook and related implementation artifacts.

## Standard Workflow

1. Sync with the target branch before starting work.
2. Create a focused topic branch using the branching strategy.
3. Make small, reviewable commits with clear messages.
4. Run relevant checks before opening a pull request.
5. Open a pull request with summary, testing, risks, and affected documents.
6. Address review comments with additional commits or clearly explained changes.
7. Merge only after required approvals and checks are complete.

## Commit Message Guidance

Use concise imperative messages, such as:

- `Expand business analysis documentation`
- `Add API error response standard`
- `Update deployment readiness checklist`

## Pull Request Checklist

- [ ] Change is scoped to a clear purpose.
- [ ] Summary explains what changed and why.
- [ ] Testing section lists exact checks performed.
- [ ] Documentation is updated when behavior, standards, or decisions change.
- [ ] No secrets, credentials, or sensitive data are included.
