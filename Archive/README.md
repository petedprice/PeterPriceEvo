# Peter Price — evolutionary genomics site

A single-page site (`index.html`, no build step) ready for GitHub Pages, plus your CV
(`Peter_Price_CV.pdf`) which the "CV (PDF)" link in the Contact section points to.

## 1. Check the content

The site is already filled in with your real bio, research areas, publications (from your CV
and Google Scholar), talks/training, and contact links. Skim through `index.html` and update
anything that changes — new papers, talks, or affiliation — by editing the relevant section
directly (each is clearly marked with an HTML comment-free block: About, Research, Publications,
Talks & training, Contact).

If you'd rather swap the CV file, just replace `Peter_Price_CV.pdf` with a new PDF of the same
filename (or update the link in the Contact section if you rename it).

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
