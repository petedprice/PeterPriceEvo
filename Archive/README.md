# Your evolutionary biology site

A single-page site (`index.html`, no build step) ready for GitHub Pages.

## 1. Customize the content

Open `index.html` and edit:
- Your name (in the header `.brand` and the hero heading)
- The hero paragraph, About section, and the "field-list" facts (position, institution, PhD year, focal system, methods)
- The three research cards in the Research section
- The Publications list (title, authors, journal, and the `href="#"` links — point them at your real paper/data/code links)
- Field notes (or delete the section if you don't want it)
- Contact links: replace `mailto:you@university.edu` and the `#` links with your real email, Google Scholar, GitHub, etc.

## 2. Put it on GitHub

```bash
# from inside this folder
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-USERNAME.github.io.git
git push -u origin main
```

Two options for the repo name:

- **`YOUR-USERNAME.github.io`** → site is live instantly at `https://YOUR-USERNAME.github.io`
- **Any other repo name** (e.g. `evo-bio-site`) → go to the repo's **Settings → Pages**, set
  Source = "Deploy from a branch", Branch = `main` / `root`, and save. Site will be live at
  `https://YOUR-USERNAME.github.io/evo-bio-site/`

Either way, it can take a minute or two for the first deploy to go live.

## 3. Custom domain (optional)

If you have your own domain (e.g. from a university or a registrar), add a file named `CNAME`
containing just your domain, and point your domain's DNS at GitHub Pages per
[GitHub's custom domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

## Notes

- Everything is in one file (`index.html`) with inline CSS — no build tools, no dependencies
  beyond two Google Fonts loaded via `<link>`.
- It's responsive (check the mobile nav toggle) and keyboard-focusable.
- To add more pages (e.g. a full CV page or per-paper pages), just add more `.html` files and
  link to them from the nav.
