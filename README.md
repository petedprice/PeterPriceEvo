# Peter Price — evolutionary genomics site

A multi-page site, no build step, ready for GitHub Pages.

## Files

- `index.html` — Home: brief intro, About, Contact
- `research.html` — Research areas, Talks & training
- `publications.html` — Full publication list
- `styles.css` — shared stylesheet used by all three pages
- `Peter_Price_CV.pdf` — your CV, linked from the footer/contact on every page

## Editing content

Each page is plain HTML — open the relevant file and edit the text directly. Shared styling
(colours, fonts, layout) lives in `styles.css`, so changing it there updates all three pages
at once. Navigation and footer contact links are duplicated across the three HTML files
(there's no templating), so if you add/rename a page, update the `<nav>` block and the footer
`<p>` in all three files to match.

## Publish / update on GitHub

```bash
# from inside this folder, after replacing the old files with these
git add .
git commit -m "Split site into separate pages"
git push
```

Since the repo is already set up and pushed once, this just updates what's live.
