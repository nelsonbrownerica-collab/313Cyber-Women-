---
title: "AI-Assisted Alert Summarizer"
date: 2026-11-25
summary: "Build a tool that turns synthetic security alerts into structured summaries for human review. It must preserve source facts, flag uncertainty, and never make autonomous response decisions."
tags:
  - "AI & Automation"
  - "Guided Lab"
authors:
  - me
featured: false
status: "Planned"
role: "Independent guided build"
duration: "15–25 hours"
---
<div class="lab-hero">
  <span class="lab-status">● PLANNED BUILD</span>
  <span class="lab-level">Advanced</span>
  <span class="lab-duration">15–25 hours</span>
</div>

> **Portfolio status:** This is a guided build plan, not a claim that the application is already implemented. Change the status only after you have completed the work and saved evidence.

## Project overview

Build a tool that turns synthetic security alerts into structured summaries for human review. It must preserve source facts, flag uncertainty, and never make autonomous response decisions.

**Suggested stack:** Python, FastAPI, Pydantic, local mock model or optional API

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

### Step 1. Define safe scope

Write a one-page scope: summarize synthetic alerts only, no automatic blocking, no live endpoint access, and human review required.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 2. Create sample alerts

Write 10 fictional alerts with timestamps, host labels, event type, severity, and evidence snippets. Avoid real IPs or personal data.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 3. Create the Python project

Set up a virtual environment, FastAPI, Pydantic, pytest, and folders for schemas, services, samples, and tests.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 4. Define a strict input schema

Validate required fields, maximum text length, timestamps, and allowed severity values. Reject unexpected fields where appropriate.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 5. Build a deterministic baseline

Before adding AI, create a rules-based summary that lists facts, missing fields, and next verification questions.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 6. Add an optional model adapter

Put model access behind one service interface. Keep keys in environment variables and never commit `.env` files. The app must still work in mock mode.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 7. Constrain the output format

Require JSON fields for summary, observed facts, uncertainty, suggested checks, and source references. Treat alert text as untrusted input.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 8. Defend against prompt injection

Do not follow instructions embedded in alert content. Separate system instructions from evidence and test malicious-looking sample strings.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 9. Add source traceability

For each statement, retain the alert field or evidence snippet that supports it. If unsupported, label it as an inference or omit it.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 10. Build a review screen

Show original alert beside the generated summary, with approve, edit, and reject controls. No action is taken on the underlying system.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 11. Evaluate quality

Create a small test set and score factual consistency, missing evidence, unsupported claims, and schema validity. Record failure examples.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 12. Document limitations

Save architecture, threat model, prompt-injection tests, evaluation results, screenshots, and a statement that analysts must verify every summary.

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
