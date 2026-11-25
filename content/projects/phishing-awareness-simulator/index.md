---
title: "Phishing Awareness Learning Simulator"
date: 2026-11-25
summary: "An offline learning app that presents fictional email examples and teaches users to identify suspicious signals without sending messages."
tags:
  - "Frontend"
  - "Security Tools"
authors:
  - me
featured: false
status: "Planned"
role: "Independent project build"
duration: "To be determined"
---
## Build status

**Planned — not implemented yet.** This page is a build brief. Do not describe the application as live, deployed, production-ready, or completed until you have built and tested it yourself.

## Project goal

An offline learning app that presents fictional email examples and teaches users to identify suspicious signals without sending messages.

## What to build

Build a safe interactive quiz using made-up emails, fake domains, and harmless placeholder links.

## Suggested technology stack

HTML, CSS, JavaScript, local JSON, optional React.

Choose the smallest stack that runs comfortably on your computer. You can start with local JSON/CSV files and SQLite; cloud services and paid APIs are not required.

## Step-by-step build plan

1. 1. Write 8 fictional email scenarios. 2. Tag each with signals such as urgency, sender mismatch, unusual request, or attachment bait. 3. Create a quiz screen. 4. Let learners select clues before seeing feedback. 5. Explain each answer in plain language. 6. Track score locally without collecting identity data. 7. Add keyboard and screen-reader support. 8. Test scoring and feedback logic.

## Data model and interfaces

Static scenario JSON; quiz state stored locally. No email sending, credential forms, or live phishing URLs.

## Acceptance criteria

- [ ] All examples are fictional
- [ ] no credential collection
- [ ] scoring is correct
- [ ] feedback explains clues
- [ ] keyboard navigation works.

## Evidence to save

- [ ] Screenshots
- [ ] scenario JSON
- [ ] quiz test results
- [ ] accessibility notes
- [ ] README.

## Suggested repository structure

```text
phishing-awareness-simulator/
├── README.md
├── docs/
│   ├── architecture.md
│   ├── test-plan.md
│   └── screenshots/
├── src/
├── tests/
└── sample-data/
```

Adapt this structure to the framework you actually choose. Do not commit secrets, private records, or real customer data.

## Final README checklist

- [ ] Explain the problem and intended users.
- [ ] List the features actually implemented.
- [ ] Document setup and run commands that have been tested.
- [ ] Describe architecture and important design decisions.
- [ ] Include screenshots or a short demo of your own application.
- [ ] Include automated test results and known limitations.
- [ ] Add a security and privacy section.
- [ ] Link to a live demo only if it genuinely exists.

## Definition of done

Move this project from **Planned** to **In Progress** when you begin implementation. Mark it **Completed** only after the working code, tests, screenshots, documentation, and limitations are committed to the repository. The starter brief itself is not evidence that the application has been built.
