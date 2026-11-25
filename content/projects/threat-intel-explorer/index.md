---
title: "Threat Intelligence Explorer"
date: 2026-11-25
summary: "Create a read-only explorer for curated public threat intelligence. Never probe, scan or contact listed infrastructure."
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

<div class="lab-meta"><span>● PLANNED</span><span>Advanced</span><span>16–26 hours</span></div>

> **Status:** This is a guided build plan, not a claim that the application is implemented. Update status only after you complete the work and save evidence.

## Project overview

Create a read-only explorer for curated public threat intelligence. Never probe, scan or contact listed infrastructure.

**Suggested tools:** Python, Flask, SQLite, STIX/TAXII concepts

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

Set a read-only scope. Never ping, browse to or otherwise interact with indicators. Defang values in reports.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 2: Plan the workflow

Review STIX concepts: indicator, malware, threat actor, campaign, relationship and report.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 3: Build the core feature

Create synthetic indicators such as hxxps://example[.]invalid/path and documentation IP ranges.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 4: Add validation and safety

Design tables for indicators, sources, sightings, tags and relationships. Track source and confidence.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 5: Test the implementation

Build a JSON importer validating type, value, source, confidence and dates.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 6: Document and capture evidence

Normalize and defang URL/domain values. Keep indicators non-clickable and do not trigger network lookups.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 7: Document and capture evidence

Build search and filters by type, source, tag, confidence and date with result limits.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 8: Document and capture evidence

Create relationship views connecting fictional campaigns, infrastructure and malware. Separate facts from hypotheses.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 9: Document and capture evidence

Show provenance on every record: source, retrieval date, confidence and handling notes.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 10: Document and capture evidence

Add local analyst notes without asserting unverified attribution as fact.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 11: Document and capture evidence

Test that indicators are not clickable, no network lookups occur and malformed imports are rejected.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 12: Document and capture evidence

Save relationship diagram, sample data, source log, screenshots, tests and an assessment with confidence caveats.

**Checkpoint:** Save a note or screenshot showing this step works.

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

- **Runtime command not found:** reopen terminal and verify the runtime version.
- **Dependency installation fails:** check runtime version and install only required packages.
- **App will not start:** read the first error, verify file paths and ports, then fix one issue at a time.
- **API errors:** inspect status and sanitized response; verify request format and required fields.
- **Tests fail:** reproduce one failure, compare expected and actual values, then rerun the suite.

## Definition of done

Mark **In Progress** when implementation begins. Mark **Completed** only after the working app, tests, screenshots, documentation and limitations are committed. A plan or mockup alone is not completion evidence.
