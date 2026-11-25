---
title: "File Integrity Checker"
date: 2026-11-25
summary: "Build a local tool that records hashes of files in a test folder and reports additions, changes and removals."
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

<div class="lab-meta"><span>● PLANNED</span><span>Beginner</span><span>6–10 hours</span></div>

> **Status:** This is a guided build plan, not a claim that the application is implemented. Update status only after you complete the work and save evidence.

## Project overview

Build a local tool that records hashes of files in a test folder and reports additions, changes and removals.

**Suggested tools:** Python standard library, hashlib, pathlib, JSON

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

Create a dedicated test folder containing harmless text files you created. Do not monitor system folders.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 2: Plan the workflow

Create main.py, baseline.json and tests. Use Python standard library only.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 3: Build the core feature

Calculate SHA-256 hashes with hashlib and stream files in chunks.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 4: Add validation and safety

Add a baseline command that records relative paths, sizes and hashes to JSON.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 5: Test the implementation

Add a verify command reporting unchanged, modified, new and missing files.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 6: Document and capture evidence

Handle permission errors and missing paths safely. Prevent symlinks escaping the chosen test folder.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 7: Document and capture evidence

Add a scope check requiring an explicit folder path inside your test workspace.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 8: Document and capture evidence

Print a concise summary and optionally export CSV.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 9: Document and capture evidence

Test changed content, new file, deleted file, empty folder and unreadable file.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 10: Document and capture evidence

Document that hashes detect change but do not prove who changed a file or that a baseline is trustworthy.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 11: Document and capture evidence

Save terminal output, sample JSON, test results and a baseline-versus-current diagram.

**Checkpoint:** Save a note or screenshot showing this step works.
### Step 12: Document and capture evidence

Commit README, usage examples, safety notes and limitations. Never include personal documents.

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
