# OS FAT Papers

Static site for the BCSE303L Operating Systems FAT papers. No build step.

- `index.html` holds all the CSS and JS. Paper data is the `const P=[...]` array near the bottom.
- `img/` has the page scans, `pdf/` the original PDFs.

## Run locally
Open `index.html` in a browser, or run `python3 -m http.server` in this folder.

## Publish on GitHub Pages
1. Push this folder to a repository.
2. Settings → Pages → Deploy from a branch → `main` / root.
3. Open `https://<user>.github.io/<repo>/`.

## Add a paper
1. Save its pages as `img/CODE-YY-YY-1.jpg`, `-2.jpg`, and so on, and its PDF as `pdf/CODE-YY-YY.pdf`.
2. Add an object to `P` with `pages` (src, w, h), `q` (question number → [page, y]) and the colour name.
   `y` is how far down the page the question starts, from 0 to 1.

Keys: `/` focus search, `←` `→` or `j` `k` change paper.
