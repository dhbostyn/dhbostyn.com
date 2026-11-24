# dhbostyn.com

Personal academic website of Dries H. Bostyn. Plain HTML and CSS: no build step and nothing to install. Hosted for free on GitHub Pages.

## Files
| File | What it is |
|---|---|
| `index.html` | Home: bio, research themes, open-science note |
| `publications.html` | Full publication list, grouped by year |
| `cv.html` | Short CV + download of the extended CV |
| `contact.html` | Email, office, profile links |
| `404.html` | "Page not found" page |
| `assets/style.css` | The one stylesheet for all pages (colours at the top) |
| `assets/` | Mouse logo, favicon |
| `files/` | PDFs: extended CV, papers, poster |

The header and footer are copied into every page. If you change the menu, change it in all five `.html` files.

## Common updates
- **Add a paper:** in `publications.html`, copy one `<li class="pub">…</li>` block, paste it at the top of the right year, and edit it. Remove link buttons you don't have. The green `class="osf"` button is for OSF data/materials/code. Or ask Claude Code: "add this paper: <reference + DOI + OSF link>".
- **New CV:** export it to PDF and overwrite `files/bostyn-cv-extended.pdf` (keep the filename so links keep working). Update `cv.html` if positions changed.
- **Add a PDF:** put it in `files/` and link to it as `files/<name>.pdf`.

## Preview locally
```
python -m http.server 8000
```
Then open http://localhost:8000. (In Claude Code: the "site" entry in `.claude/launch.json`.)

## Publish
Commit and push to the `main` branch on GitHub. GitHub Pages republishes automatically within a minute or two.

## Not in this repo
`old-site-archive/` (the recovered Wix site) and `START-PROMPT.md` stay local only (see `.gitignore`). The repo is public, so don't commit anything private.
