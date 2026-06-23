# davidepafumi.github.io

Personal academic website of **Davide Pafumi** — PhD candidate in English and
Digital Humanities at the University of Lethbridge.

Built with plain [Jekyll](https://jekyllrb.com/) and hosted on GitHub Pages.
It was originally based on the [al-folio](https://github.com/alshedivat/al-folio)
theme but has been rebuilt as a lightweight, dependency-light site.

## Run locally

```bash
bundle install
bundle exec jekyll serve
```

Then open <http://localhost:4000>.

## Structure

- `_pages/` — about (home), publications, projects, cv, teaching, blog index
- `_posts/` — blog posts ("unsolicited")
- `_projects/` — research project pages
- `_data/socials.yml` — social / academic profile links
- `_layouts/`, `_includes/` — minimal HTML templates
- `assets/css/style.css` — hand-written stylesheet (no framework)
- `assets/img/`, `assets/pdf/` — images and CV
