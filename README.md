# fateme-pourghasem.github.io

Personal academic and professional portfolio for **Fateme Pourghasem**, built with the [**al-folio**](https://github.com/alshedivat/al-folio) Jekyll theme.

**Live site:** [https://fateme-pourghasem.github.io](https://fateme-pourghasem.github.io) (after GitHub Pages deploy)

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`.

## Customize

- **Identity & SEO:** `_config.yml` (set `email` when you want it shown; `url` must match your GitHub Pages domain).
- **Bio (home):** `_pages/about.md`
- **Publications:** `_bibliography/papers.bib` (also tune `scholar` section in `_config.yml`).
- **CV blocks:** `_data/cv.yml`
- **GitHub cards:** `_data/repositories.yml`
- **Project cards:** `_projects/*.md`
- **Profile photo:** replace `assets/img/prof_pic.jpg` with your headshot (same filename).

## Deploy

Push the `main` (or `master`) branch to **`Fateme-pourghasem/Fateme-pourghasem.github.io`**. Enable **GitHub Pages** from GitHub Actions (workflow `Deploy site` is included).

Upstream theme: [alshedivat/al-folio](https://github.com/alshedivat/al-folio).
