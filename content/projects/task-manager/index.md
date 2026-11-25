---
title: "Secure Task & Workflow Manager"
date: 2026-11-25
summary: "Build a task board with projects, due dates, task ownership, comments, and role-aware access. Use fictional users and local development data."
tags:
  - "Web Applications"
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
  <span class="lab-level">Intermediate</span>
  <span class="lab-duration">15–25 hours</span>
</div>

> **Portfolio status:** This is a guided build plan, not a claim that the application is already implemented. Change the status only after you have completed the work and saved evidence.

## Project overview

Build a task board with projects, due dates, task ownership, comments, and role-aware access. Use fictional users and local development data.

**Suggested stack:** Vue or React, Node.js, Express, SQLite, CSS

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

### Step 1. Create the project

Create a repository and folders for frontend, backend, tests, and docs. Record the problem and three user roles: viewer, member, and administrator.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 2. Design the data model

Define users, projects, tasks, and comments. Use stable IDs, timestamps, status values, and foreign keys.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 3. Build the board interface

Create columns for To Do, In Progress, and Done. Add task cards with title, due date, priority, and owner.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 4. Add task creation and editing

Build forms with required-field checks, length limits, and clear validation messages.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 5. Build the backend API

Create endpoints to list, create, update, and delete tasks. Validate every request on the server.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 6. Add role permissions

Define a permission matrix. Viewers can read; members can update assigned tasks; administrators can manage project members. Enforce rules in backend middleware.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 7. Add filters and search

Filter by status, priority, owner, and due date. Search titles without injecting raw user input into SQL.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 8. Add activity history

Record task changes with timestamp, actor ID, and changed fields. Do not store passwords or session tokens in activity logs.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 9. Add notifications

Start with in-app notifications or a local mock. Avoid sending real emails until opt-in and privacy handling are designed.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 10. Test authorization boundaries

Verify a viewer cannot edit, a member cannot alter another user's restricted task, and an unauthenticated request is rejected.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 11. Test usability

Check mobile layout, keyboard access, form labels, empty states, and clear error messages.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 12. Publish documentation

Save schema diagram, permission matrix, screenshots, API examples, test results, setup steps, and known limitations.

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
