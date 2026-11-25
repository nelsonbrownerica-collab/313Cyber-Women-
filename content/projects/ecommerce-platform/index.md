---
title: "Secure E-Commerce Application"
date: 2026-11-25
summary: "Build a local storefront with a product catalog, search, cart, mock checkout, order history, and a small admin area. Use test data and simulated payments only."
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
<div class="lab-hero">
  <span class="lab-status">● PLANNED BUILD</span>
  <span class="lab-level">Intermediate</span>
  <span class="lab-duration">20–30 hours</span>
</div>

> **Portfolio status:** This is a guided build plan, not a claim that the application is already implemented. Change the status only after you have completed the work and saved evidence.

## Project overview

Build a local storefront with a product catalog, search, cart, mock checkout, order history, and a small admin area. Use test data and simulated payments only.

**Suggested stack:** React, Node.js, Express, SQLite, CSS, GitHub Actions

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

### Step 1. Prepare the workspace

Install Node.js LTS and VS Code. Create a GitHub repository named secure-ecommerce. Create client, server, docs, and tests folders. Run `git init` and add a README.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 2. Plan the user journeys

Sketch visitor, customer, and admin flows. Write user stories for browse, search, add-to-cart, checkout simulation, and product maintenance. Define what is out of scope: real payments and real customer accounts.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 3. Create sample data

Add 8–12 fictional products in a JSON file. Give each an ID, name, description, price in cents, category, and stock count. Never store prices as floating-point values.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 4. Build the catalog UI

Create responsive product cards, search, category filters, and an empty-state message. Check keyboard navigation and mobile layout.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 5. Create the API

Add `GET /api/products`, `GET /api/products/:id`, and `GET /api/health`. Validate IDs and return consistent JSON errors.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 6. Add cart behavior

Support add, remove, and quantity changes. Reject zero, negative, non-integer, and over-stock quantities. Recalculate totals on the server.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 7. Add a simulated checkout

Create `POST /api/orders` that accepts a test cart only. Re-read product prices on the server, calculate totals, and return a fake order number. Do not collect card numbers or connect payment services.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 8. Add account-flow demonstration

Use clearly labeled demo accounts or a local mock login. If implementing real password storage, hash passwords with a maintained password-hashing library and never log credentials.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 9. Create the admin view

Allow a demo admin to add, edit, and deactivate sample products. Validate all fields on the server and document role checks.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 10. Test important cases

Test valid cart totals, stock limits, invalid quantities, missing products, malformed requests, and checkout with an empty cart.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 11. Review security and accessibility

Check input validation, output escaping, safe error messages, dependency audit output, focus order, labels, and color contrast.

**Checkpoint:** Save a screenshot or short note showing this step works.

### Step 12. Document and publish evidence

Add setup instructions, architecture sketch, API examples, test output, screenshots, and limitations. Deploy only if you can configure it safely; never add secrets to Git.

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
