# prof-daniel-read.github.io

Personal academic website, built by GitHub Pages with Jekyll. No build tools are needed on your computer — edit a file on GitHub (pencil icon), commit, and the site rebuilds in a minute or two.

Live at <https://prof-daniel-read.github.io>.

## Files

| File | What it is |
|---|---|
| `_config.yml` | Site title, email, ORCID, Google Scholar, photo, CV PDF, and the navigation menu |
| `index.md` | Home page (bio + recent work) |
| `publications.md` | Full publication list |
| `cv.md` | CV page (positions, education, grants, reports, teaching) |
| `pdfs/` | Paper PDFs linked from the publications page |
| `assets/style.css` | Look and feel |
| `_layouts/default.html` | Page template shared by all pages (header, menu, footer) |

## Common edits

- **Add a photo:** upload it as `assets/photo.jpg`, then set `photo: /assets/photo.jpg` in `_config.yml`.
- **Add a CV PDF:** upload it as `assets/cv.pdf`, then set `cv_pdf: /assets/cv.pdf` in `_config.yml`. Download links appear on the home and CV pages.
- **Show email / Google Scholar:** fill in `email:` or `google_scholar:` in `_config.yml`. Empty values are hidden.
- **Add a publication:** copy a line in `publications.md`, edit it, keep newest first. To link a PDF, upload it to `pdfs/` and add `[PDF](/pdfs/FILENAME.pdf)`.

## Adding a page

1. Create e.g. `research.md`:

   ```
   ---
   layout: default
   title: Research
   permalink: /research/
   ---

   # Research

   Your text here.
   ```

2. Add a matching entry under `nav:` in `_config.yml`.
