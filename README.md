# TithiShop - Bengali Ethnic Foods (Quarto Site)

A Quarto-powered website to showcase authentic Bengali ethnic foods and connect with the community. Edit pages with simple Markdown; Quarto builds the HTML for GitHub Pages.

## What's Included

- `_quarto.yml` — site configuration (theme, navbar, output to `docs/`)
- `index.qmd` — homepage with About, Products, Contact
- `styles.css` — small style tweaks
- `index.html` — earlier static version (optional; Quarto uses `index.qmd`)

## Prerequisites

- Install Quarto: see `https://quarto.org/docs/get-started/`

## Local Preview

```bash
quarto preview
```

This starts a local server with live reload.

## Build for GitHub Pages

This project is configured to output the site to the `docs/` folder.

```bash
quarto render
```

Commit and push the generated `docs/` folder.

## Publish to GitHub Pages

1. Create a new public repository on GitHub (e.g., `TithiShop`)
2. Push this project to the repo:
   ```bash
   git init
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/TithiShop.git
   git add .
   git commit -m "Initial Quarto site for TithiShop"
   git push -u origin main
   ```
3. In GitHub → Settings → Pages:
   - Source: Deploy from a branch
   - Branch: `main` / folder: `/docs`
4. Your site will be at: `https://YOUR_USERNAME.github.io/TithiShop/`

Alternatively, you can use:

```bash
quarto publish gh-pages
```

(This creates a `gh-pages` branch automatically. You may need a GitHub token.)

## Customize Content

Edit `index.qmd` using Markdown:

```markdown
## Our Products

- 🥭 Mango Pickle (আমের আচার)
  - Traditional Bengali mango pickle with mustard oil and spices.
```

Update contact info in the Contact section:
- Replace `your-email@example.com`
- Replace `+1 (234) 567-890`
- Add your social links

## Notes

- If you use the Quarto flow, GitHub Pages should serve from `docs/`. The legacy `index.html` is not required.
- If you prefer not to render locally, enable GitHub Actions for Quarto builds (see Quarto docs).

---

Made with ❤️ for the Bengali Community

