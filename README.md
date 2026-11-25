# 313 Cyber Women — Software Developer Portfolio

A custom static portfolio for Erica Nelson. This website is built with plain HTML, CSS, and JavaScript and deploys directly to GitHub Pages.

## Technology
- HTML5
- CSS3
- Vanilla JavaScript
- GitHub Pages with GitHub Actions

## Local preview
Open `index.html` in a browser, or run a simple local server from the repository root:

```powershell
py -m http.server 8000
```

Then open `http://localhost:8000`.

## Project explorer
The portfolio includes 11 project build guides. Every guide is marked **Planned** until the application is implemented and its evidence is committed. Each guide includes setup, numbered steps, testing, evidence, deliverables, troubleshooting, and a definition of done.

## Deployment
Every push to `main` runs `.github/workflows/deploy.yml`, packages the static site, and deploys it to GitHub Pages. No Hugo, Go, Node, package manager, theme, or build step is required.

## Repository structure
- `index.html` — portfolio homepage
- `static/css/` — custom visual theme
- `static/js/` — navigation and project filters
- `projects/` — standalone project guide pages
- `content/projects/` — original Markdown source copies of the project guides
- `assets/media/authors/me.png` — profile portrait source
- `static/uploads/resume.pdf` — resume file

## Accuracy
Project status is not represented as completed without implementation evidence. Portfolio copy avoids invented employment, credentials, and project claims.
