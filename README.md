# Mario Qosja – Academic Homepage

Personal academic website served via GitHub Pages at **https://qosmar.github.io**.

## Contents

| File / Dir | Purpose |
|---|---|
| `index.html` | Single-page homepage (HTML + embedded CSS) |
| `cv.pdf` | Compiled CV (linked from the "Download CV" button) |
| `cv.tex` | LaTeX source for the CV |
| `img/` | Site assets (profile photo, etc.) |

## Updating the site

1. Edit `index.html` locally.
2. If you change `cv.tex`, recompile:
   ```bash
   pdflatex cv.tex && pdflatex cv.tex   # run twice for references
   ```
3. Commit and push:
   ```bash
   git add -A
   git commit -m "Update …"
   git push origin main
   ```

GitHub Pages picks up the change automatically (usually < 1 min).

## No build step

The site is pure static HTML/CSS — no framework, no bundler, no server-side code.
