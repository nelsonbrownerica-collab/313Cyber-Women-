---
title: "Phishing Awareness Simulator"
date: 2026-11-25
summary: "Create a local educational quiz that teaches users to spot suspicious messages. It does not send emails, collect credentials, track real users, or imitate a real organization."
tags:
  - "Security Tools"
  - "Guided Lab"
authors:
  - me
featured: false
status: "Planned"
role: "Independent guided build"
duration: "8–14 hours"
---
<div class="lab-hero">
  <span class="lab-status">● PLANNED BUILD</span>
  <span class="lab-level">Beginner</span>
  <span class="lab-duration">8–14 hours</span>
</div>

> **Portfolio status:** This is a guided build plan, not a claim that the application is already implemented. Change the status only after you have completed the work and saved evidence.

## Project overview

Create a local educational quiz that teaches users to spot suspicious messages. It does not send emails, collect credentials, track real users, or imitate a real organization.

**Suggested stack:** HTML, CSS, JavaScript, local JSON

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

### Step 1. Set the learning goals

Choose 5–8 concepts: sender mismatch, urgency, suspicious links, unexpected attachments, requests for secrets, and reporting.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 2. Create a static project

Create index.html, styles.css, app.js, and a fictional examples.json file. Use no external tracking scripts.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 3. Write fictional examples

Create safe sample messages with fictional brands and reserved example domains. Include both suspicious and legitimate examples.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 4. Build the message viewer

Display sender, subject, message body, and link text. Make all links inert; do not navigate to external destinations.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 5. Add answer choices

Ask learners to identify warning signs and choose a safe next step. Do not ask for passwords or personal information.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 6. Explain each answer

After selection, explain the indicators and why the safe action is to verify through a trusted channel.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 7. Add progress and scoring

Track score only in browser memory or local storage. Provide a reset button and disclose what is stored.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 8. Add accessibility

Use semantic headings, keyboard-accessible controls, visible focus, and accessible feedback announcements.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 9. Test the scenarios

Check every example, correct answer, explanation, reset, and mobile layout.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 10. Review privacy

Confirm there is no analytics, credential collection, external email, or network submission.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 11. Capture evidence

Save screenshots, example dataset, test checklist, and README.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 12. Write a facilitator note

Explain that this is an educational simulation and should never be used to trick or shame participants.

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
