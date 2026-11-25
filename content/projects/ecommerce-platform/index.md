---
title: "Secure E-Commerce Application"
date: 2026-11-25
summary: "Build a local storefront with product catalog, search, cart, simulated checkout, order history and admin product management."
tags:
  - "Web Applications"
  - "Guided Lab"
authors:
  - me
featured: false
status: "Planned"
role: "Independent guided build"
duration: "20–30 hours"
---

<div class="lab-meta"><span>● PLANNED</span><span>Intermediate</span><span>20–30 hours</span></div>

> **Status:** This is a guided build plan, not a claim that the application is implemented. Update the status only after you complete the work and save evidence.

## Project overview

Build a local storefront with product catalog, search, cart, simulated checkout, order history and admin product management.

**Suggested tools:** React, Node.js, Express, SQLite

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

Create a GitHub repository and folders for client, server, tests, docs and sample-data. Install Node.js LTS and verify node and npm versions.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 2: Plan the workflow

Sketch customer and admin journeys. Define product, cart, order and demo-user fields. Store prices as integer cents.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 3: Build the core feature

Create fictional product seed data in JSON with ID, name, category, priceCents and stock.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 4: Add validation and safety

Build responsive product cards, search, category filters, loading and empty states. Use semantic HTML and keyboard controls.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 5: Test the implementation

Create GET /api/products and GET /api/products/:id. Validate IDs and return consistent JSON errors.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 6: Document and capture evidence

Implement cart add/remove/quantity behavior. Reject non-integer, zero, negative and over-stock quantities.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 7: Document and capture evidence

Implement POST /api/orders in test mode only. Recalculate prices and totals server-side; return a mock order ID. Never request payment credentials.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 8: Document and capture evidence

Create a demo admin product form. Validate fields on the server and document role checks.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 9: Document and capture evidence

Test cart totals, invalid quantities, missing products, empty checkout and stock limits.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 10: Document and capture evidence

Review input validation, output escaping, error messages, dependency audit, focus order and color contrast.

**Checkpoint:** Save a short note or screenshot showing this step works.
### Step 11: Document and capture evidence

Document setup, architecture, API examples, screenshots, test output, security notes and known limitations.

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
