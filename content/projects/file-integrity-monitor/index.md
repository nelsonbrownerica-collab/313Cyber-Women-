---
title: "File Integrity Checker"
date: 2026-11-25
summary: "Build a local tool that records cryptographic hashes of files in a test folder and reports additions, changes, and removals. Never run it against system folders or files you do not own."
tags:
  - "Python"
  - "Guided Lab"
authors:
  - me
featured: false
status: "Planned"
role: "Independent guided build"
duration: "6–10 hours"
---
<div class="lab-hero">
  <span class="lab-status">● PLANNED BUILD</span>
  <span class="lab-level">Beginner</span>
  <span class="lab-duration">6–10 hours</span>
</div>

> **Portfolio status:** This is a guided build plan, not a claim that the application is already implemented. Change the status only after you have completed the work and saved evidence.

## Project overview

Build a local tool that records cryptographic hashes of files in a test folder and reports additions, changes, and removals. Never run it against system folders or files you do not own.

**Suggested stack:** Python standard library, hashlib, pathlib, JSON

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

### Step 1. Create a safe test folder

Make a project folder with a monitored-sample directory containing copies of harmless text files you created.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 2. Create the Python environment

Use Python 3 and the standard library. Create main.py, baseline.json, and tests.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 3. Calculate SHA-256 hashes

Use hashlib and stream files in chunks. Record relative paths, file sizes, and SHA-256 digests.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 4. Create a baseline command

Add a command that writes the current inventory to JSON. Require an explicit folder path.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 5. Create a verify command

Compare current hashes to the baseline and report unchanged, modified, new, and missing files.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 6. Handle errors safely

Handle permission errors and missing paths without crashing. Do not follow symlinks outside the chosen test directory.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 7. Add an allowlisted scope

Resolve paths and verify each target remains inside the selected test folder.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 8. Add readable output

Print a concise summary and optionally export a CSV report.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 9. Write automated tests

Test changed content, new file, deleted file, empty folder, and unreadable file behavior.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 10. Document limitations

Explain that hashes detect change but do not prove who changed a file or whether a baseline is trustworthy.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 11. Capture evidence

Save terminal output, sample JSON, test results, and a diagram of baseline-versus-current comparison.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 12. Commit the project

Add README, usage examples, safety notes, and known limitations. Never include personal documents or sensitive files.

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
