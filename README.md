# hemenhosseini.github.io

Source of my personal website: **https://hemenhosseini.github.io/**

Built with Jekyll and deployed automatically by GitHub Actions (`.github/workflows/jekyll-gh-pages.yml`)
on every push to `main`. You can edit everything directly on github.com — no local setup needed.

## Where to edit things

| What | File |
|---|---|
| Name, email, social links, photo/CV switches | `_config.yml` |
| About text on the home page | `index.html` |
| Research description | `research.md` |
| **Publications** | `_data/publications.yml` (template inside) |
| **Projects** | `_data/projects.yml` |
| News items on the home page | `_data/news.yml` |
| CV (positions, education, skills) | `_data/cv.yml` |
| **Articles / blog posts** | `_posts/YYYY-MM-DD-title.md` |
| Colours & fonts | `assets/css/style.css` (`--accent` at the top) |

### Add an article
Create `_posts/2026-12-01-my-article.md`:

```markdown
---
layout: post
title: "My article"
summary: "One-sentence summary shown in the list."
tags: [spectroscopy]
---

Text in Markdown. LaTeX works: $$E = \hbar\omega$$
```

### Add a photo or CV PDF
- Photo: upload a square image as `assets/img/profile.jpg`, then set `show_photo: true` in `_config.yml`.
- CV: upload `assets/files/cv.pdf`, then set `cv_pdf: true`.
- Paper PDFs: put them in `assets/files/` and reference them with `pdf: /assets/files/name.pdf`.

## Preview locally (optional)
```bash
gem install jekyll jekyll-feed jekyll-seo-tag
jekyll serve
```
