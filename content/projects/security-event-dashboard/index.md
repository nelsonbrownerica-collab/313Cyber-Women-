---
title: "Security Event Dashboard"
date: 2026-11-25
summary: "A lightweight dashboard that imports synthetic security events and displays event counts, severity, timelines, and filters."
tags:
  - "Python"
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

A lightweight dashboard that imports synthetic security events and displays event counts, severity, timelines, and filters.

## What to build

Build an offline dashboard for sample authentication and endpoint events; no real organization logs are needed.

## Suggested technology stack

Python, CSV/JSON, SQLite, Streamlit or Flask, Plotly (optional).

Choose the smallest stack that runs comfortably on your computer. You can start with local JSON/CSV files and SQLite; cloud services and paid APIs are not required.

## Step-by-step build plan

1. 1. Create synthetic CSV fields: timestamp, user, host, event_type, result, source. 2. Validate and normalize records. 3. Store data in SQLite or load read-only. 4. Calculate event totals and failed-login trends. 5. Add date, user, and severity filters. 6. Display a timeline and top categories. 7. Add malformed-row handling. 8. Export a sanitized summary report.

## Data model and interfaces

Tables: events, users (synthetic). Views: totals, event trend, filtered event table. Optional endpoint: GET /api/events.

## Acceptance criteria

- [ ] Dashboard works from sample data
- [ ] malformed rows reported
- [ ] filters match query results
- [ ] no personal or employer data.

## Evidence to save

- [ ] Synthetic CSV
- [ ] dashboard screenshots
- [ ] SQL/schema
- [ ] test cases
- [ ] exported report
- [ ] README.

## Suggested repository structure

```text
security-event-dashboard/
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
