---
title: "Incident Response Case Manager"
date: 2026-11-25
summary: "A case-tracking application for documenting fictional security incidents, evidence references, timelines, owners, and response tasks."
tags:
  - "Full-Stack"
  - "Security Tools"
authors:
  - me
featured: false
status: "Planned"
role: "Independent project build"
duration: "To be determined"
---
## Build status

**Planned — not implemented yet.** This page is a build brief. Do not describe the application as live, deployed, production-ready, or completed until you have built and tested it yourself.

## Project goal

A case-tracking application for documenting fictional security incidents, evidence references, timelines, owners, and response tasks.

## What to build

Build a simple case workspace with status tracking and an audit trail using fictional cases only.

## Suggested technology stack

React, Node.js/Express, SQLite, CSS, GitHub Actions.

Choose the smallest stack that runs comfortably on your computer. You can start with local JSON/CSV files and SQLite; cloud services and paid APIs are not required.

## Step-by-step build plan

1. 1. Define case lifecycle: new, triage, investigating, contained, resolved, closed. 2. Design case, event, evidence_reference, and task tables. 3. Build case list and detail pages. 4. Add timeline entries with UTC timestamps. 5. Add evidence references by filename/hash only. 6. Add role-aware updates and audit history. 7. Add filters and export to Markdown/JSON. 8. Test lifecycle and access rules.

## Data model and interfaces

Cases, timeline_events, evidence_refs, response_tasks, audit_events. API: GET/POST /api/cases, POST /api/cases/:id/events.

## Acceptance criteria

- [ ] Lifecycle transitions validated
- [ ] timeline ordered
- [ ] evidence references contain no actual sensitive files
- [ ] audit history retained.

## Evidence to save

- [ ] Screenshots
- [ ] ERD
- [ ] API docs
- [ ] sample fictional case export
- [ ] tests
- [ ] README.

## Suggested repository structure

```text
incident-case-manager/
├── README.md
├── docs/
│   ├── architecture.md
│   ├── test-plan.md
│   └── screenshots/
├── src/
├── tests/
└── sample-data/
```

Adapt this structure to the framework you actually choose. Do not commit secrets, private records, or real customer data.

## Final README checklist

- [ ] Explain the problem and intended users.
- [ ] List the features actually implemented.
- [ ] Document setup and run commands that have been tested.
- [ ] Describe architecture and important design decisions.
- [ ] Include screenshots or a short demo of your own application.
- [ ] Include automated test results and known limitations.
- [ ] Add a security and privacy section.
- [ ] Link to a live demo only if it genuinely exists.

## Definition of done

Move this project from **Planned** to **In Progress** when you begin implementation. Mark it **Completed** only after the working code, tests, screenshots, documentation, and limitations are committed to the repository. The starter brief itself is not evidence that the application has been built.
