# Pratik's Agent Gallery

A static GitHub Pages site showcasing pre-built M365 Copilot & Copilot Studio agents, inspired by the [Microsoft M365 Agent Templates](https://microsoft.github.io/m365-agent-templates/) gallery.

**Live site:** https://pratikbhusal18.github.io

## Featured Agents

1. **Document Validation Agent** — Pratik Bhusal
2. **PowerClaw** — Alejandro Lopez

Both pulled from the M365 Copilot Technical Center of Excellence — Agent Repository.

## Local preview

Open `index.html` directly in any browser, or run:

```powershell
python -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages

```powershell
cd "C:\Users\prbhusal\OneDrive - Microsoft\Documents\Clawpilot\pratikbhusal18.github.io"
git init
git add .
git commit -m "Initial agent gallery"
git branch -M main
git remote add origin https://github.com/pratikbhusal18/pratikbhusal18.github.io.git
git push -u origin main
```

Then in your repo on GitHub: **Settings → Pages → Source: `main` / root**. Site goes live at `https://pratikbhusal18.github.io` within a minute or two.

> The `<username>.github.io` repo name is special — GitHub serves it at the root of your user subdomain automatically. If you'd rather use a different repo name (e.g., `agent-gallery`), the site will be served at `https://pratikbhusal18.github.io/agent-gallery/`.

## Files

```
.
├── index.html                   # The gallery page
├── assets/
│   ├── document-validation.svg  # Tile icon for Document Validation Agent
│   ├── powerclaw.svg            # Tile icon for PowerClaw
│   └── favicon.svg              # Browser favicon
└── README.md
```

## Customize

- Add a new agent: copy an `<article class="card">` block in `index.html` and update the icon, title, tagline, and links.
- Change the theme: edit the CSS variables at the top of `index.html` (`--accent`, `--bg`, etc.).
