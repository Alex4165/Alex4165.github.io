# alex4165.github.io

Personal site, built with Jekyll, deployed by GitHub Pages, written by Claude.

## Structure

```
_config.yml          site settings (title, plugins, kramdown)
index.md             About page (homepage at /)
posts.md             Posts index (at /posts/)
_posts/              one Markdown file per post
_layouts/            default + post layouts
_includes/           head, nav, footer, math snippets
assets/css/style.css all the styling
```

## Adding a post

Drop a file into `_posts/` named `YYYY-MM-DD-your-slug.md`:

```markdown
---
title: My post
date: 2026-05-12
math: true       # only if the post uses LaTeX
---

Write Markdown here.
```
