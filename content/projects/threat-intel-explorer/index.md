---
title: "Threat Intelligence Indicator Explorer"
date: 2026-11-25
summary: "An offline explorer for fictional threat indicators and their relationships to reports, campaigns, and defensive recommendations."
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

An offline explorer for fictional threat indicators and their relationships to reports, campaigns, and defensive recommendations.

## What to build

Build a searchable local catalog of defanged indicators using synthetic data; focus on data modeling and provenance.

## Suggested technology stack

Python, JSON, SQLite, Streamlit or Flask.

Choose the smallest stack that runs comfortably on your computer. You can start with local JSON/CSV files and SQLite; cloud services and paid APIs are not required.

## Step-by-step build plan

1. 1. Create synthetic indicators with defanged domains/IPs/hashes. 2. Add source, first_seen, last_seen, confidence, and context. 3. Store records in SQLite. 4. Build search and filters. 5. Link indicators to fictional reports and behaviors. 6. Add confidence and expiry labels. 7. Export a sanitized intelligence brief. 8. Test duplicate handling and stale indicator warnings.

## Data model and interfaces

Indicators, reports, relationships tables. Indicator values remain defanged text and are never resolved or contacted.

## Acceptance criteria

- [ ] Provenance visible
- [ ] duplicate records handled
- [ ] expired items flagged
- [ ] no outbound indicator lookup or automatic blocking.

## Evidence to save

- [ ] Data dictionary
- [ ] screenshots
- [ ] synthetic dataset
- [ ] export sample
- [ ] tests
- [ ] README.

## Suggested repository structure

```text
threat-intel-explorer/
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
