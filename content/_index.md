---
title: ""
summary: "Software development portfolio featuring practical, security-aware applications and guided build projects."
date: 2026-11-25
type: landing

sections:
  - block: dev-hero
    id: hero
    content:
      username: me
      greeting: "Hi, I'm"
      show_status: true
      show_scroll_indicator: true
      typewriter:
        enable: true
        prefix: "I build"
        strings:
          - "practical software tools"
          - "security-aware web applications"
          - "Python and data projects"
          - "AI-assisted workflows"
        type_speed: 65
        delete_speed: 35
        pause_time: 2200
      cta_buttons:
        - text: Explore My Projects
          url: "#projects"
          icon: arrow-down
        - text: Open the Build Guides
          url: "/projects/"
          icon: code
    design:
      style: centered
      avatar_shape: circle
      animations: true
      background:
        color:
          light: "#fafafa"
          dark: "#0a0a0f"
      spacing:
        padding: ["6rem", "0", "4rem", "0"]

  - block: portfolio
    id: projects
    content:
      title: "Cybersecurity Software Projects"
      subtitle: "Ten software builds designed to develop practical application-development skills through security-minded tools."
      count: 10
      filters:
        folders:
          - projects
      buttons:
        - name: All Projects
          tag: "*"
        - name: Security Tools
          tag: Security Tools
        - name: Full-Stack
          tag: Full-Stack
        - name: Python
          tag: Python
        - name: AI
          tag: AI
      default_button_index: 0
    design:
      columns: 3
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  - block: tech-stack
    id: skills
    content:
      title: "Development Toolkit"
      subtitle: "Technologies used or being explored across the project builds—not a claim that every tool is already mastered."
      categories:
        - name: Languages & Data
          items:
            - name: Python
              icon: devicon/python
            - name: JavaScript
              icon: devicon/javascript
            - name: SQL
              icon: devicon/mysql
        - name: Web Development
          items:
            - name: HTML5
              icon: devicon/html5
            - name: CSS3
              icon: devicon/css3
            - name: React
              icon: devicon/react
            - name: Node.js
              icon: devicon/nodejs
        - name: Tools & Workflow
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
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  - block: cta-card
    id: about
    content:
      title: "A developer portfolio built around real progress"
      text: |
        313 Cyber Women is my software development portfolio. The projects here are build plans and learning challenges until I complete them, test them, and publish my own evidence.

        My approach is to build in small steps, explain the decisions, test the important paths, document what works, and keep improving the code.
      button:
        text: Browse All Build Guides
        url: "/projects/"
        new_tab: false
    design:
      card:
        css_class: "bg-gradient-to-br from-primary-200 via-primary-100 to-secondary-200 dark:from-primary-600 dark:via-primary-700 dark:to-secondary-700"
        text_color: dark
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "5rem", "0"]

  - block: contact-info
    id: contact
    content:
      title: "Connect & Collaborate"
      subtitle: "Follow the code and project progress"
      text: |
        Interested in a project or want to follow the development process? Visit my GitHub profile to explore the repositories and updates.
      email: ""
      autolink: false
    design:
      columns: "1"
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
---
