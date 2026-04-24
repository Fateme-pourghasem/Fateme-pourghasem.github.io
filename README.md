# fateme-pourghasem.github.io

Personal academic and professional portfolio for **Faye Pourghasem**, built with the [**al-folio**](https://github.com/alshedivat/al-folio) Jekyll theme.

**Live site:** [https://fateme-pourghasem.github.io](https://fateme-pourghasem.github.io)

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

## Deploy (GitHub Pages)

The workflow **Deploy site** (`.github/workflows/deploy.yml`) runs Jekyll on GitHub Actions and pushes the built HTML to the **`gh-pages`** branch. That branch is what must be served as the website.

If you see **“404 There isn’t a GitHub Pages site here”**, the deploy likely succeeded but **Pages is pointed at the wrong source**:

1. Open the repo on GitHub → **Settings** → **Pages** (left sidebar).
2. Under **Build and deployment** → **Source**, choose **Deploy from a branch** (not “GitHub Actions” for this setup).
3. **Branch:** select **`gh-pages`** → folder **`/` (root)** → **Save**.
4. Wait one or two minutes, then open [https://fateme-pourghasem.github.io/](https://fateme-pourghasem.github.io/) again.

**Do not** set the source to **`main`**: GitHub’s built-in Jekyll cannot build al-folio (plugins like `jekyll-scholar`), so the site will stay broken or 404.

After each push to `main`, check **Actions** → **Deploy site** is green; then Pages will update from `gh-pages`.

Upstream theme: [alshedivat/al-folio](https://github.com/alshedivat/al-folio).
