# Fuyao Huang Academic Website

This website uses the official [al-folio](https://github.com/alshedivat/al-folio) Jekyll project.

## Where to update content

- Personal introduction and portrait settings: `_pages/about.md`
- Site title, theme features, search, and blog settings: `_config.yml`
- Email and GitHub profile: `_data/socials.yml`
- GitHub cards: `_data/repositories.yml`
- Publications: `_bibliography/papers.bib`
- Blog posts: add Markdown files to `_posts/` using the name `YYYY-MM-DD-title.md`
- Pink theme: `_sass/_themes.scss`
- Portrait: `assets/img/fuyao-huang.jpg`

## Add a blog post

Create `_posts/2026-09-06-example-title.md`:

```markdown
---
layout: post
title: Example title
date: 2026-09-06
description: A one-sentence summary.
tags: machine-learning biology
categories: research-notes
---

Write the post here.
```

## Add a publication

Append a normal BibTeX entry to `_bibliography/papers.bib`. Useful optional fields include:

- `abbr`: short venue name
- `html`: paper page
- `code`: code repository
- `selected = {true}`: also show the paper on the home page

## Local preview

The official recommended workflow is Docker:

```bash
docker compose pull
docker compose up
```

Then open `http://localhost:8080/`.

If Ruby 3.3 and Bundler are already installed, use:

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000/`.

## GitHub Pages

For the personal address `https://yaoaoy.github.io`, create a repository named `YaoaoY.github.io`, upload this source to its `main` branch, enable GitHub Actions, and configure Pages to publish from the generated `gh-pages` branch.
