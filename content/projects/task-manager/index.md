---
title: "Secure Task & Workflow Manager"
date: 2026-11-25
summary: "A task management app with user roles, project boards, due dates, audit history, and permission checks."
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

A task management app with user roles, project boards, due dates, audit history, and permission checks.

## What to build

Build a responsive task board where demo users can create and update tasks within their assigned workspace.

## Suggested technology stack

React, Node.js/Express, SQLite, CSS, GitHub Actions.

Choose the smallest stack that runs comfortably on your computer. You can start with local JSON/CSV files and SQLite; cloud services and paid APIs are not required.

## Step-by-step build plan

1. 1. Define roles: owner, editor, viewer. 2. Design users/projects/tasks schema. 3. Build sign-in simulation or local demo accounts. 4. Add task CRUD and status transitions. 5. Enforce authorization on the server for every operation. 6. Add audit events for task changes. 7. Build board and list views. 8. Test cross-user access denial and document results.

## Data model and interfaces

Users, workspaces, memberships, tasks, audit_events. API: GET/POST /api/tasks, PATCH /api/tasks/:id, GET /api/audit-events.

## Acceptance criteria

- [ ] Viewer cannot edit
- [ ] user cannot access another workspace
- [ ] required fields validated
- [ ] audit history records changes.

## Evidence to save

- [ ] Role matrix
- [ ] screenshots
- [ ] API tests
- [ ] sample audit log
- [ ] architecture notes
- [ ] README.

## Suggested repository structure

```text
task-manager/
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
