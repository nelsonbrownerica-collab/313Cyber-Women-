---
title: ""
summary: "Erica Nelson's software development portfolio: secure applications, Python automation, APIs, and AI-assisted tools."
date: 2026-11-25
type: landing

sections:
  - block: dev-hero
    id: hero
    content:
      username: me
      greeting: "SOFTWARE DEVELOPER & CYBER INNOVATOR"
      show_status: false
      show_scroll_indicator: true
      typewriter:
        enable: true
        prefix: "BUILDING SECURE SOLUTIONS."
        strings:
          - "CREATING IMPACT."
          - "DEVELOPING WITH PURPOSE."
          - "DESIGNING SECURITY-MINDED SOFTWARE."
        type_speed: 55
        delete_speed: 28
        pause_time: 2100
      cta_buttons:
        - text: Explore Projects
          url: "#projects"
          icon: code
        - text: View My Resume
          url: "/uploads/resume.pdf"
          icon: download
    design:
      style: centered
      avatar_shape: circle
      animations: true
      background:
        color:
          light: "#F8FAFC"
          dark: "#030712"
      spacing:
        padding: ["4rem", "0", "2rem", "0"]

  - block: portfolio
    id: projects
    content:
      title: "Explore My Projects"
      subtitle: "Choose a build guide to open its step-by-step lab, tools, testing plan, troubleshooting notes, evidence checklist, and final deliverables."
      count: 11
      filters:
        folders:
          - projects
      buttons:
        - name: All Projects
          tag: "*"
        - name: Web Applications
          tag: Web Applications
        - name: Security Tools
          tag: Security Tools
        - name: APIs & Integrations
          tag: APIs & Integrations
        - name: AI & Automation
          tag: AI & Automation
        - name: Python
          tag: Python
        - name: Data & Analytics
          tag: Data & Analytics
      default_button_index: 0
    design:
      columns: 3
      background:
        color:
          light: "#FFFFFF"
          dark: "#030712"
      spacing:
        padding: ["2rem", "0", "4rem", "0"]

  - block: tech-stack
    id: skills
    content:
      title: "Tools & Technologies"
      subtitle: "Tools used or explored across the guided builds. Each project lists its own setup requirements."
      categories:
        - name: Programming & Data
          items:
            - name: Python
              icon: devicon/python
            - name: JavaScript
              icon: devicon/javascript
            - name: SQL
              icon: devicon/mysql
        - name: Web & APIs
          items:
            - name: HTML5
              icon: devicon/html5
            - name: CSS3
              icon: devicon/css3
            - name: React
              icon: devicon/react
            - name: Node.js
              icon: devicon/nodejs
        - name: Developer Workflow
          items:
            - name: GitHub
              icon: brands/github
            - name: GitHub Actions
              icon: brands/github
            - name: VS Code
              icon: devicon/vscode
            - name: SQLite
              icon: devicon/sqlite
    design:
      style: grid
      show_levels: false
      background:
        color:
          light: "#F1F5F9"
          dark: "#071426"
      spacing:
        padding: ["3rem", "0", "3rem", "0"]

  - block: cta-card
    id: about
    content:
      title: "Security-minded development. Practical results."
      text: |
        I build and document practical applications with attention to clean code, user needs, secure design, testing, and clear technical documentation.

        Each project guide includes a build sequence, testing steps, troubleshooting notes, and an evidence checklist. Project status stays transparent: planned work is not presented as completed work.
      button:
        text: Browse All Project Guides
        url: "/projects/"
        new_tab: false
    design:
      background:
        color:
          light: "#F1F5F9"
          dark: "#071426"
      spacing:
        padding: ["3rem", "0", "4rem", "0"]

  - block: contact-info
    id: contact
    content:
      title: "Let's Connect"
      subtitle: "Explore the code and follow project progress"
      text: |
        Visit my GitHub profile to explore source code, project documentation, and future releases.
      email: ""
      autolink: false
    design:
      columns: "1"
      background:
        color:
          light: "#FFFFFF"
          dark: "#030712"
      spacing:
        padding: ["3rem", "0", "4rem", "0"]
---
