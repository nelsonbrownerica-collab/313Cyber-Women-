---
title: "Security Event Dashboard"
date: 2026-11-25
summary: "Build a dashboard that imports synthetic security events, normalizes fields, filters events and visualizes trends. Do not upload employer or personal logs."
tags:
  - "Security Tools"
  - "Guided Lab"
authors:
  - me
featured: false
status: "Planned"
role: "Independent guided build"
duration: "18–28 hours"
---

<div class="lab-meta"><span>● PLANNED</span><span>Intermediate</span><span>18–28 hours</span></div>

> **Status:** This is a guided build plan, not a claim that the application is implemented. Update the status only after you complete the work and save evidence.

## Project overview

Build a dashboard that imports synthetic security events, normalizes fields, filters events and visualizes trends. Do not upload employer or personal logs.

**Suggested tools:** Python, Flask, SQLite, Chart.js

## Learning objectives

- Plan a small application and explain its architecture.
- Build and validate its main workflow.
- Test normal, invalid and edge-case behavior.
- Document security, privacy, accessibility and limitations.
- Present reproducible evidence of your own implementation.

## Before you begin

Use fictional sample data. Work only in a dedicated project folder and on systems you own. Keep passwords, tokens and API keys out of source control. Start with the smallest local setup that works on your computer.

## Tools and setup

1. Install the runtime and editor listed above.
2. Create a GitHub repository for this project.
3. Clone it locally and open the folder in your editor.
4. Add a README, .gitignore, and folders for source code, tests, sample data and docs.
5. Record tool versions in the README.
6. Run a minimal starter app and confirm it works before adding features.

## Step-by-step lab guide

### Step 1: Set up the workspace

Create a Python virtual environment and install Flask and a database library. Add app, sample-data, tests and docs folders.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 2: Plan the workflow

Generate fictional CSV/JSON events. Use documentation IP ranges and fictional usernames.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 3: Build the core feature

Define normalized fields: timestamp, event_id, user, source_ip, event_type, severity and summary.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 4: Add validation and safety

Build an importer that validates fields, normalizes timestamps to UTC and reports malformed rows.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 5: Test the implementation

Store events in SQLite with indexes. Use parameterized queries.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 6: Document and capture evidence

Create routes for dashboard summaries and filtered events. Limit results and validate date ranges.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 7: Document and capture evidence

Build charts for event volume, severity distribution and top event types using Chart.js.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 8: Document and capture evidence

Add drill-down details with escaped output and a visible synthetic-data label.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 9: Document and capture evidence

Add a documented educational rule for repeated failed logins; do not call it a production detection.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 10: Document and capture evidence

Test malformed timestamps, missing fields, duplicates, empty data and filters.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 11: Document and capture evidence

Capture sample data, schema diagram, importer report, dashboard screenshots, test output and README.

**Checkpoint:** Save a short note or screenshot showing this step works.

## Testing checklist

- [ ] App starts using documented commands.
- [ ] Main workflow works with fictional sample data.
- [ ] Invalid and missing inputs are handled safely.
- [ ] Errors do not expose secrets or stack traces.
- [ ] Keyboard navigation and mobile layout are checked.
- [ ] Automated tests pass or manual results are documented.
- [ ] Dependencies and configuration are reviewed.

## Evidence checklist

- [ ] GitHub repository with readable source code.
- [ ] Screenshot of the working application.
- [ ] Setup and run output.
- [ ] Architecture or data-flow diagram.
- [ ] Test plan and test results.
- [ ] Example input/output using fictional data.
- [ ] README with setup, features, limitations and security notes.

## Final deliverables

1. Source code in GitHub.
2. README with tested setup instructions.
3. Tests and results.
4. Screenshots or a short demo.
5. Architecture notes and known limitations.
6. A reflection describing what you learned and what you would improve.

## Troubleshooting

- **Runtime command not found:** reopen the terminal and verify the runtime version.
- **Dependency installation fails:** check the runtime version and install only required packages.
- **App will not start:** read the first error, verify file paths and ports, then fix one issue at a time.
- **API errors:** inspect status and sanitized response; verify request format and required fields.
- **Tests fail:** reproduce one failure, compare expected and actual values, then rerun the suite.

## Definition of done

Mark **In Progress** when implementation begins. Mark **Completed** only after the working app, tests, screenshots, documentation and limitations are committed. A plan or mockup alone is not completion evidence.
