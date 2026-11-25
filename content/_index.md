---
title: ""
summary: "Erica Nelson's software development portfolio: practical applications, Python automation, secure APIs, and AI-assisted tools."
date: 2026-11-25
type: landing

sections:
  - block: dev-hero
    id: hero
    content:
      username: me
      greeting: "Hello, I'm"
      show_status: false
      show_scroll_indicator: true
      typewriter:
        enable: true
        prefix: "I develop"
        strings:
          - "security-minded software"
          - "Python automation tools"
          - "web applications and APIs"
          - "AI-assisted workflows"
        type_speed: 65
        delete_speed: 35
        pause_time: 2200
      cta_buttons:
        - text: Explore My Projects
          url: "#projects"
          icon: arrow-down
        - text: View Source Code
          url: "https://github.com/nelsonbrownerica-collab"
          icon: brands/github
    design:
      style: centered
      avatar_shape: circle
      animations: true
      background:
        color:
          light: "#F8FAFC"
          dark: "#050B16"
      spacing:
        padding: ["6rem", "0", "4rem", "0"]

  - block: portfolio
    id: projects
    content:
      title: "Selected Software Projects"
      subtitle: "Practical builds focused on application development, secure-by-design thinking, automation, and AI. Each project page explains the build plan and current status."
      count: 11
      filters:
        folders:
          - projects
      buttons:
        - name: All Projects
          tag: "*"
        - name: Full-Stack
          tag: Full-Stack
        - name: Python
          tag: Python
        - name: Security Tools
          tag: Security Tools
        - name: AI
          tag: AI
      default_button_index: 0
    design:
      columns: 3
      background:
        color:
          light: "#FFFFFF"
          dark: "#071426"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  - block: tech-stack
    id: skills
    content:
      title: "Technologies & Development Workflow"
      subtitle: "Tools selected for the projects in this portfolio. Project pages identify what is planned and what has actually been implemented."
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
        - name: Developer Tools
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
          dark: "#050B16"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  - block: cta-card
    id: about
    content:
      title: "How I approach building software"
      text: |
        I focus on practical applications with clear user needs, thoughtful architecture, input validation, access controls, useful tests, and readable documentation.

        My process is to define the problem, build in manageable steps, test expected and unexpected behavior, document technical decisions, and improve the result. This portfolio is a transparent record of that work—not a list of skills or products I haven't demonstrated.
      button:
        text: Browse All Build Guides
        url: "/projects/"
        new_tab: false
    design:
      card:
        css_class: "bg-gradient-to-br from-blue-100 via-slate-100 to-cyan-100 dark:from-blue-950 dark:via-slate-900 dark:to-cyan-950"
        text_color: dark
      background:
        color:
          light: "#F1F5F9"
          dark: "#071426"
      spacing:
        padding: ["4rem", "0", "5rem", "0"]

  - block: contact-info
    id: contact
    content:
      title: "Connect"
      subtitle: "Explore the code and follow project progress"
      text: |
        For project details and source code, visit my GitHub profile. Each completed project will include its own repository, documentation, tests, and supporting evidence.
      email: ""
      autolink: false
    design:
      columns: "1"
      background:
        color:
          light: "#FFFFFF"
          dark: "#050B16"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
---
