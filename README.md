# Personal website

A minimal Jekyll site for GitHub Pages. No build tools needed on your computer — GitHub builds it.

## Files

| File | What it is |
|---|---|
| `_config.yml` | Site title, email, and the navigation menu |
| `index.md` | Home page (bio + photo) |
| `cv.md` | CV page |
| `assets/photo.jpg` | Your photo — add this |
| `assets/cv.pdf` | Your CV PDF — add this |
| `assets/style.css` | Look and feel |
| `_layouts/default.html` | Page template shared by all pages (header, menu, footer) |

## Publishing (one time)

1. On GitHub, create a new repository named **`yourusername.github.io`** (replace with your GitHub username). Make it public.
2. Upload all these files, keeping the folders (drag the contents of this folder onto the repo's "Add file → Upload files" page).
3. Add `assets/photo.jpg` and `assets/cv.pdf`.
4. Go to **Settings → Pages**, and under "Build and deployment" choose **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
5. After a minute or two the site is live at `https://yourusername.github.io`.

If you name the repo something else (e.g. `website`), the site appears at `https://yourusername.github.io/website/` instead; everything still works.

## Editing

Edit any `.md` file directly on GitHub (pencil icon) and commit. The site rebuilds automatically.

## Adding a page

1. Create `research.md`:

   ```
   ---
   layout: default
   title: Research
   permalink: /research/
   ---

   # Research

   Your text here.
   ```

2. Uncomment (or add) the matching lines under `nav:` in `_config.yml`.

## Custom domain (optional)

Settings → Pages → Custom domain, then follow GitHub's instructions for your DNS provider.
