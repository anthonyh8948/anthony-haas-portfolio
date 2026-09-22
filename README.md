# Anthony Haas — Portfolio Site

A static, single-page portfolio site (no build step, no dependencies) covering education, experience, ventures, skills, and contact info.

## Structure

```
index.html
assets/
  css/styles.css
  js/main.js
  resume/Anthony-Haas-Resume.docx
```

## Run locally

Any static server works, e.g.:

```bash
cd anthony-haas-portfolio
python3 -m http.server 8000
```

Then open http://localhost:8000

## Editing content

All copy lives directly in `index.html` — sections are labeled with HTML comments (`<!-- HERO -->`, `<!-- EXPERIENCE -->`, etc.). Colors and fonts are defined as CSS variables at the top of `assets/css/styles.css` under `:root`.

To update the downloadable résumé, replace `assets/resume/Anthony-Haas-Resume.docx` with a new file of the same name (or update the `href` in the hero section of `index.html`).

## Deploying

**Vercel / Netlify (recommended, free):**
1. Push this folder to a GitHub repo.
2. Import the repo in Vercel or Netlify — no build command needed, it's static HTML.
3. Optionally attach a custom domain.

**GitHub Pages:**
1. Push to a GitHub repo.
2. Repo Settings → Pages → deploy from the `main` branch, root folder.

## Custom domain

Once deployed, buying something like `anthonyhaas.com` or `tonyhaas.dev` and pointing it at the host gives you a clean URL to put on your résumé and LinkedIn.
