---
title: "File Integrity Checker"
date: 2026-11-25
summary: "A local utility that calculates SHA-256 hashes for user-selected benign files and compares them with a saved manifest."
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

A local utility that calculates SHA-256 hashes for user-selected benign files and compares them with a saved manifest.

## What to build

Build a read-only integrity checker for a dedicated sample folder; it must never modify monitored files.

## Suggested technology stack

Python standard library: hashlib, pathlib, json, argparse, unittest.

Choose the smallest stack that runs comfortably on your computer. You can start with local JSON/CSV files and SQLite; cloud services and paid APIs are not required.

## Step-by-step build plan

1. 1. Create a folder with harmless text samples. 2. Write a function to stream files and calculate SHA-256. 3. Generate a JSON baseline manifest. 4. Compare current files with the manifest. 5. Report added, changed, and missing files. 6. Add command-line options for folder and manifest paths. 7. Handle unreadable files safely. 8. Add unit tests for unchanged/changed/missing files.

## Data model and interfaces

CLI commands: baseline and verify. Manifest stores relative path, size, and SHA-256.

## Acceptance criteria

- [ ] Read-only behavior
- [ ] deterministic output
- [ ] missing/changed files identified
- [ ] tests pass
- [ ] no unknown binaries executed.

## Evidence to save

- [ ] Python source
- [ ] manifest sample
- [ ] terminal screenshots
- [ ] unit test output
- [ ] README.

## Suggested repository structure

```text
file-integrity-monitor/
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
