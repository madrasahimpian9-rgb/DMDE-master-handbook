# Testing Guide

## Purpose

Testing guidance defines how DMDE changes are validated before release. Testing should cover correctness, security, integration behavior, data quality, and operational readiness.

## Test Types

| Test Type | Purpose |
| --- | --- |
| Unit tests | Validate small units of domain or application behavior. |
| Integration tests | Validate interactions with databases, services, queues, or external adapters. |
| Contract tests | Validate API and event compatibility between producers and consumers. |
| End-to-end tests | Validate critical workflows from a user or system perspective. |
| Security tests | Validate authentication, authorization, data protection, and abuse cases. |
| Performance tests | Validate response time, throughput, and resource usage under expected load. |
| Documentation checks | Validate Markdown formatting, links, examples, and required sections. |

## Test Planning

- Link tests to requirements, business rules, risks, and acceptance criteria.
- Prioritize tests for high-risk workflows and sensitive data paths.
- Include negative cases, boundary cases, and permission cases.
- Record manual validation steps when automation is not available.

## Pull Request Testing Notes

Each pull request should list exact commands or checks run and explain any skipped checks or environment limitations.
