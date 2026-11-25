---
title: "Incident Response Case Manager"
date: 2026-11-25
summary: "Build a local case-management app for fictional incidents with timeline, evidence register, tasks and report export."
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

<div class="lab-meta"><span>● PLANNED</span><span>Advanced</span><span>18–28 hours</span></div>

> **Status:** This is a guided build plan, not a claim that the application is implemented. Update status only after you complete the work and save evidence.

## Project overview

Build a local case-management app for fictional incidents with timeline, evidence register, tasks and report export.

**Suggested tools:** Python, Flask, SQLite, HTML/CSS, CSV export

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

Map intake, triage, investigation, containment recommendation, recovery and lessons learned. App records decisions; it does not perform containment.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 2: Plan the workflow

Define cases, events, evidence items, tasks, notes and users with timestamps and references.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 3: Build the core feature

Build a case list showing ID, title, severity, status, owner and last update.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 4: Add validation and safety

Create intake fields for summary, fictional asset, discovery time, severity and reporter role.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 5: Test the implementation

Build a timeline for dated observations and actions. Preserve original entries and record edits.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 6: Document and capture evidence

Create an evidence register with evidence ID, description, source, collection time, SHA-256, custodian and storage reference. Do not upload actual evidence files.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 7: Document and capture evidence

Add investigation tasks with owner, due date and status. Separate facts from hypotheses.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 8: Document and capture evidence

Define viewer, analyst and administrator roles and enforce permissions on the server.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 9: Document and capture evidence

Export a case summary with timeline, evidence register, open questions, decisions and lessons learned.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 10: Document and capture evidence

Test edit history, role boundaries, missing evidence metadata, invalid timestamps and report export.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 11: Document and capture evidence

Use fictional data, sanitize exports and document that chain-of-custody requirements vary.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 12: Document and capture evidence

Save screenshots, data model, sample report, tests, README and fictional walkthrough.

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
