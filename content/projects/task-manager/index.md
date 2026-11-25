---
title: "Secure Task & Workflow Manager"
date: 2026-11-25
summary: "Build a task board with projects, task ownership, due dates, comments, activity history and role-aware access using fictional users."
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

<div class="lab-meta"><span>● PLANNED</span><span>Intermediate</span><span>15–25 hours</span></div>

> **Status:** This is a guided build plan, not a claim that the application is implemented. Update the status only after you complete the work and save evidence.

## Project overview

Build a task board with projects, task ownership, due dates, comments, activity history and role-aware access using fictional users.

**Suggested tools:** Vue or React, Node.js, Express, SQLite

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

Create a repository and frontend, backend, tests and docs folders. Define viewer, member and administrator roles.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 2: Plan the workflow

Design users, projects, tasks and comments tables with IDs, timestamps, status values and foreign keys.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 3: Build the core feature

Build a responsive board with To Do, In Progress and Done columns and task cards.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 4: Add validation and safety

Add create/edit forms with required fields, length limits and validation messages.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 5: Test the implementation

Build API routes to list, create, update and delete tasks. Validate input server-side.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 6: Document and capture evidence

Create a permission matrix and enforce access rules in backend middleware, not only in the interface.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 7: Document and capture evidence

Add search and filters for status, priority, owner and due date. Use parameterized database queries.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 8: Document and capture evidence

Record activity history with actor, timestamp and changed fields. Never log passwords or tokens.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 9: Document and capture evidence

Add local in-app notification mockups; do not send email or expose user data.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 10: Document and capture evidence

Test role boundaries, invalid input, empty states, keyboard navigation and mobile layout.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 11: Document and capture evidence

Save screenshots, schema diagram, permission matrix, API examples, test results and README.

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
