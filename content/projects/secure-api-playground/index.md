---
title: "Secure REST API Playground"
date: 2026-11-25
summary: "Build a small API with validation, authentication concepts, safe error handling, and automated tests. Run locally with synthetic data."
tags:
  - "APIs & Integrations"
  - "Guided Lab"
authors:
  - me
featured: false
status: "Planned"
role: "Independent guided build"
duration: "12–20 hours"
---
<div class="lab-hero">
  <span class="lab-status">● PLANNED BUILD</span>
  <span class="lab-level">Intermediate</span>
  <span class="lab-duration">12–20 hours</span>
</div>

> **Portfolio status:** This is a guided build plan, not a claim that the application is already implemented. Change the status only after you have completed the work and saved evidence.

## Project overview

Build a small API with validation, authentication concepts, safe error handling, and automated tests. Run locally with synthetic data.

**Suggested stack:** Python FastAPI or Node.js Express, SQLite, pytest

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

### Step 1. Choose the stack

Choose either FastAPI with Pydantic or Express with a validation library. Keep the first version local.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 2. Define resources

Model a simple notes or inventory resource with ID, title, body, owner, and timestamps.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 3. Create CRUD endpoints

Implement list, read, create, update, and delete routes. Return consistent status codes and JSON.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 4. Validate input

Set field types, length limits, allowed values, and request-size limits. Reject unexpected or malformed input.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 5. Use parameterized database access

Create SQLite tables and use bound parameters. Do not concatenate user input into SQL.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 6. Add authentication safely

Use a local test token or maintained auth library. Store secrets in environment variables and never log tokens.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 7. Enforce authorization

Check that a user can only read or modify resources they own unless an administrator role is explicitly allowed.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 8. Add rate-limit and CORS configuration

Use a conservative local development policy and document production settings separately.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 9. Harden error handling

Return generic client errors while keeping sanitized diagnostic logs. Do not expose stack traces or secrets.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 10. Test security cases

Test invalid JSON, oversized fields, unauthorized access, IDOR-style ownership checks, and SQL injection-shaped text as inert input.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 11. Document the API

Add OpenAPI screenshots or schema, sample requests, test output, and a data-flow diagram.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 12. Review and publish

Run dependency checks, inspect secrets, capture evidence, and document that this is a local learning API.

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
