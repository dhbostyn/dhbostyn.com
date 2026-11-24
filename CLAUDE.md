# CLAUDE.md

Academic website for Dries H. Bostyn (dhbostyn.com). Dries is a psychologist, not a web developer: explain technical steps briefly and in plain language.

- Plain static HTML/CSS, no generator, no JavaScript, no external requests (system fonts only). Keep it that way unless Dries asks.
- Header/nav and footer are duplicated in every `.html` page; keep them in sync. `404.html` uses root-absolute paths (`/assets/...`), the other pages use relative paths.
- Publications: `publications.html`, newest year first, one `<li class="pub">` per paper (title, authors with `<b>Bostyn, D. H.</b>`, venue, link buttons). Verify DOIs resolve (`https://doi.org/api/handles/<doi>` returns 200) before adding. OSF links use `class="osf"`.
- Source for publications/positions is Dries's extended CV; the current PDF is `files/bostyn-cv-extended.pdf` (exported from his Word CV).
- Repo is PUBLIC (GitHub Pages). Never commit `old-site-archive/`, `START-PROMPT.md`, or anything private.
- Preview: `.claude/launch.json` → "site" (python http.server on :8000).
- Publishing = push to `main`; GitHub Pages serves the repo root.
- Open item: Google Scholar link (commented-out TODO in `contact.html`) awaits the profile URL from Dries. "Bright mind, moral mind" (2020) OSF link may be wrong (TODO comment in `publications.html`).
