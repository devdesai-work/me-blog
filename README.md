# Minimal Personal Blog (GitHub Pages)

A clean, minimal personal site inspired by karpathy.github.io and ready for GitHub Pages.

## Structure

- `index.md`: landing page
- `posts.md`: page listing all posts
- `_posts/`: blog post markdown files (source directory for posts)
- `_layouts/`: shared page and post templates
- `assets/css/style.css`: styling
- `assets/images/`: place post images here

## Add a post

Create a file in `_posts/`:

`YYYY-MM-DD-title.md`

Example front matter:

```md
---
title: My Post
date: 2026-05-04
image: /assets/images/my-image.jpg
---

Post content here.
```

## Deploy on GitHub Pages

1. Push this repo to GitHub.
2. In GitHub: `Settings` -> `Pages`.
3. Set source to `GitHub Actions`.
4. Push to `main` branch; `.github/workflows/pages.yml` will deploy automatically.

After deployment, update `_config.yml` `url` with your real GitHub Pages URL.
