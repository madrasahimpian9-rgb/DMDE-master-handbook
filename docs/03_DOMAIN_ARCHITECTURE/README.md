# Domain Architecture

Domain architecture defines the business-aligned boundaries, responsibilities, data ownership, workflows, integrations, and quality expectations for each DMDE domain. Each book should help product owners, analysts, architects, and delivery teams understand what a domain owns and how it collaborates with the rest of the platform.

## Domain Books

| Book | Domain | Purpose |
| --- | --- | --- |
| `Book-01-Identity-and-Access/` | Identity and Access | Manage users, authentication, authorization, roles, permissions, sessions, account lifecycle, and access audit trails. |
| `Book-02-Organization/` | Organization | Manage institution profiles, organizational hierarchy, units, departments, classes, groups, memberships, and structural context. |
| `Book-03-Academic-Structure/` | Academic Structure | Define academic years, terms, levels, programs, subjects, schedules, calendars, and academic operating structures. |
| `Book-04-Student-Management/` | Student Management | Maintain student profiles, enrollment, lifecycle status, guardians, class placement, and student record history. |
| `Book-05-Teacher-Management/` | Teacher Management | Maintain teacher profiles, assignments, workload, availability, competency mapping, and teaching responsibilities. |
| `Book-06-Curriculum/` | Curriculum | Manage curriculum structures, competencies, learning outcomes, subject mapping, and curriculum versioning. |
| `Book-07-Assessment/` | Assessment | Support assessment setup, grading rules, score capture, feedback, moderation, progress review, and result publication. |
| `Book-08-Jendela-Nilai/` | Jendela Nilai | Provide a focused grade-window experience for reviewing, validating, publishing, and communicating learner scores and progress. |
| `Book-09-Website-CMS/` | Website CMS | Manage public website content, pages, announcements, media, navigation, approvals, and publication workflows. |
| `Book-10-Dashboard-Analytics/` | Dashboard Analytics | Provide operational dashboards, analytics views, metrics, scorecards, filters, exports, and insight workflows. |
| `Book-11-Notification/` | Notification | Manage notification templates, recipients, channels, delivery rules, status tracking, and communication audit trails. |
| `Book-12-Document-Management/` | Document Management | Manage templates, generated documents, storage references, approvals, signatures, retention, and document audit history. |
| `Book-13-Public-Portal/` | Public Portal | Provide public-facing access to approved information, announcements, forms, search, and stakeholder-facing resources. |
| `Book-14-Mobile-PWA/` | Mobile PWA | Provide mobile-friendly and progressive web access to core DMDE workflows, notifications, offline-tolerant views, and quick actions. |
| `Book-15-AI-Services/` | AI Services | Provide governed AI-assisted capabilities for summarization, recommendations, content support, analytics assistance, and productivity workflows. |
| `Book-16-Reporting/` | Reporting | Manage operational reports, formal exports, reporting definitions, schedules, data lineage, and compliance evidence. |

## Standard Book Structure

Each domain book should maintain:

- Domain purpose and business outcomes.
- Ownership and stakeholder responsibilities.
- Core entities and lifecycle concepts.
- Primary workflows and business rules.
- APIs, events, integrations, and dependencies.
- Security, privacy, audit, reporting, and operational considerations.
- Open decisions, risks, and roadmap notes.

## Maintenance Guidance

- Keep domain boundaries aligned with business capabilities and enterprise architecture decisions.
- Document cross-domain dependencies explicitly instead of relying on tribal knowledge.
- Link domain rules to business rules and functional requirements where relevant.
- Add ADR or TDR references when domain design choices affect enterprise standards.
