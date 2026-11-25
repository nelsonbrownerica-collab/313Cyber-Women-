---
title: "Security Event Dashboard"
date: 2026-11-25
summary: "Create a dashboard that imports synthetic security events, normalizes fields, filters events, and visualizes trends. Use generated or public sample logs only; do not upload employer or personal logs."
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
<div class="lab-hero">
  <span class="lab-status">● PLANNED BUILD</span>
  <span class="lab-level">Intermediate</span>
  <span class="lab-duration">18–28 hours</span>
</div>

> **Portfolio status:** This is a guided build plan, not a claim that the application is already implemented. Change the status only after you have completed the work and saved evidence.

## Project overview

Create a dashboard that imports synthetic security events, normalizes fields, filters events, and visualizes trends. Use generated or public sample logs only; do not upload employer or personal logs.

**Suggested stack:** Python, Flask, SQLite, Chart.js, CSV/JSON

## Learning objectives

By completing this lab, you should be able to:

- Plan a small application and explain its architecture.
- Build and validate the core workflow.
- Test normal, invalid, and edge-case behavior.
- Document security, privacy, accessibility, and known limitations.
- Present reproducible evidence of your own implementation.

## Before you begin

- Use fictional sample data and accounts.
- Keep API keys and passwords out of source control.
- Work in a dedicated project folder; do not test against systems or data you do not own.
- Commit small changes so you can recover if something breaks.
- If your computer is low on storage, use the simplest stack and local files first.

## Tools and setup

1. Install the current stable version of the language/runtime listed above.
2. Install Visual Studio Code or another editor you already use.
3. Create a new GitHub repository for this project.
4. Clone it to your computer and open the folder in your editor.
5. Create a `README.md`, `.gitignore`, and folders for source code, tests, sample data, and documentation.
6. Record the versions of your tools in the README.
7. Run a minimal “hello world” or starter app and save the successful output before adding features.

## Step-by-step lab guide

### Step 1. Prepare the lab

Create a Python virtual environment and install Flask, pandas, and a database library. Create sample-data, app, tests, and docs folders.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 2. Generate safe sample events

Create a small CSV/JSON dataset with fictional timestamps, usernames, event types, source IPs from documentation ranges, and severities.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 3. Define a normalized schema

Map source fields into timestamp, event_id, user, source_ip, event_type, severity, and summary. Document missing or malformed values.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 4. Build the importer

Parse CSV and JSON, validate required fields, normalize timestamps to UTC, and reject malformed rows with a report.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 5. Store events locally

Use SQLite with indexes on timestamp, severity, and event type. Use parameterized queries.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 6. Create the Flask routes

Add a dashboard route and API endpoints for event counts, severity summaries, and filtered events.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 7. Build the dashboard

Use Chart.js to show event volume over time, severity distribution, and top event types.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 8. Add filters

Allow date range, severity, event type, and user filters. Validate date ranges and limit result counts.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 9. Add drill-down details

Click an event to see normalized fields and the original sample row. Escape displayed values.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 10. Add detection rules

Create simple documented rules such as repeated failed logins in a short window. Mark them as educational examples, not production detections.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 11. Test the pipeline

Test valid imports, bad timestamps, missing fields, duplicate event IDs, empty data, and filter combinations.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 12. Capture evidence

Save a sample dataset, schema diagram, importer report, dashboard screenshots, test output, and README. State clearly that all records are synthetic.

**Checkpoint:** Save a screenshot or short note showing this step works.


## Testing checklist

- [ ] The application starts using the documented command.
- [ ] The main user workflow works with sample data.
- [ ] Invalid and missing inputs are handled safely.
- [ ] Errors are understandable and do not expose secrets or stack traces.
- [ ] Keyboard navigation and mobile layout have been checked.
- [ ] Automated tests pass, or manual test results are documented.
- [ ] Dependencies and configuration have been reviewed.

## Evidence checklist

- [ ] Repository link with readable source code.
- [ ] Screenshot of the working application.
- [ ] Screenshot or text output of setup and run commands.
- [ ] Architecture or data-flow diagram.
- [ ] Test plan and test results.
- [ ] Example input and output using fictional data.
- [ ] README with setup, features, limitations, and security notes.

## Final deliverables

1. Source code in GitHub.
2. A complete README with tested setup instructions.
3. Tests and test results.
4. Screenshots or a short demonstration.
5. Architecture notes and known limitations.
6. A brief reflection describing what you learned and what you would improve.

## Troubleshooting

- **Runtime or package command not found:** close and reopen the terminal after installation, then verify the runtime version.
- **Dependency installation fails:** check the runtime version, network connection, and exact error; install only the packages this project needs.
- **Application will not start:** read the first error message, check the file path and port, and fix one issue at a time.
- **API returns an error:** inspect the status code and sanitized response; verify the request format and required fields.
- **Tests fail:** reproduce one failing test, compare expected and actual values, and rerun the full suite after fixing it.

## Definition of done

Mark **In Progress** when you begin implementation. Mark **Completed** only when the working application, tests, screenshots, documentation, and limitations are committed. A plan or generated mockup alone is not completion evidence.
