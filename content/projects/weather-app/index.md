---
title: "API-Driven Dashboard"
date: 2026-11-25
summary: "Build a responsive dashboard demonstrating API requests, loading states, error handling and data visualization. Begin with local mock JSON."
tags:
  - "APIs & Integrations"
  - "Guided Lab"
authors:
  - me
featured: false
status: "Planned"
role: "Independent guided build"
duration: "6–12 hours"
---

<div class="lab-meta"><span>● PLANNED</span><span>Beginner</span><span>6–12 hours</span></div>

> **Status:** This is a guided build plan, not a claim that the application is implemented. Update status only after you complete the work and save evidence.

## Project overview

Build a responsive dashboard demonstrating API requests, loading states, error handling and data visualization. Begin with local mock JSON.

**Suggested tools:** HTML, CSS, JavaScript, fetch API, optional public API

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

Create index.html, styles.css, app.js and data/sample-weather.json.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 2: Plan the workflow

Sketch current conditions, hourly summary and multi-day view with accessible labels and responsive cards.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 3: Build the core feature

Load local JSON and render the same structure an API would return so the project works offline.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 4: Add validation and safety

Write a fetch function using async/await, check response status and parse JSON safely.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 5: Test the implementation

Add loading, error and retry states. Do not show raw stack traces.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 6: Document and capture evidence

Validate location input with trimming and length limits; show clear errors for unsupported values.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 7: Document and capture evidence

Add Celsius/Fahrenheit units and format dates with browser APIs.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 8: Document and capture evidence

Render a temperature trend with accessible text labels; do not rely on color alone.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 9: Document and capture evidence

Cache the last successful response briefly and indicate when cached data is displayed.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 10: Document and capture evidence

Test offline mode, malformed JSON, non-200 responses, missing fields and empty input.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 11: Document and capture evidence

Check keyboard navigation, contrast, responsive cards and screen-reader labels.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 12: Document and capture evidence

Document mock mode, optional API configuration, key handling, screenshots, tests and data-source attribution.

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
