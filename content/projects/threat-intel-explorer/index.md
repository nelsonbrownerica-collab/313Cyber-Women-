---
title: "Threat Intelligence Explorer"
date: 2026-11-25
summary: "Create a read-only explorer for curated public threat-intelligence indicators and relationships. Use synthetic indicators or reputable public feeds; do not probe or contact listed infrastructure."
tags:
  - "Security Tools"
  - "Guided Lab"
authors:
  - me
featured: false
status: "Planned"
role: "Independent guided build"
duration: "16–26 hours"
---
<div class="lab-hero">
  <span class="lab-status">● PLANNED BUILD</span>
  <span class="lab-level">Advanced</span>
  <span class="lab-duration">16–26 hours</span>
</div>

> **Portfolio status:** This is a guided build plan, not a claim that the application is already implemented. Change the status only after you have completed the work and saved evidence.

## Project overview

Create a read-only explorer for curated public threat-intelligence indicators and relationships. Use synthetic indicators or reputable public feeds; do not probe or contact listed infrastructure.

**Suggested stack:** Python, Flask, SQLite, STIX/TAXII concepts, OpenCTI concepts

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

### Step 1. Set the scope and safety rules

Build a read-only research tool. Never scan, ping, browse to, or otherwise interact with indicators. Use defanged values in screenshots and reports.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 2. Learn the data model

Review STIX concepts: indicator, malware, threat actor, campaign, relationship, and report. Document the fields you plan to support.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 3. Create sample intelligence

Use synthetic indicators such as `hxxps://example[.]invalid/path` and reserved documentation IP ranges. Label all data as sample.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 4. Design the database

Create tables for indicators, sources, sightings, tags, and relationships. Track source and confidence.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 5. Build an import parser

Import a small JSON file and validate indicator type, value, source, confidence, and first/last seen dates.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 6. Normalize and defang

Normalize domain and URL strings for display. Keep potentially dangerous indicators defanged and never make them clickable.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 7. Build search and filters

Search by indicator type, source, tag, confidence, and date. Limit result sizes.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 8. Create relationship views

Show how a fictional campaign connects to infrastructure and malware records. Clearly distinguish sourced facts from analyst hypotheses.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 9. Add provenance

Every record must show source, retrieval date, confidence, and handling notes.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 10. Add analyst notes

Allow local notes and tags. Do not present unverified attribution as fact.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 11. Test safety controls

Verify that indicators are not clickable, no network lookups occur, and malformed imports are rejected.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 12. Publish an intelligence brief

Save a relationship diagram, sample dataset, source log, screenshots, tests, and a one-page assessment with confidence caveats.

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
