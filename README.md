# alex4165.github.io

Personal site, built with Jekyll, deployed by GitHub Pages.

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

Commit, push to `main`, GitHub Pages rebuilds in ~30 seconds.

## Math

KaTeX renders client-side. The script only loads on pages with `math: true` in their front matter.

- Inline: `\(x^2\)`
- Display: `$$ \int f(x)\,dx $$` or `\[ ... \]`

Use `\(...\)` for inline (not `$...$`) so plain dollar signs in prose don't get parsed as math.

## Local preview (optional)

GitHub builds the site for you on push, so you don't need this. If you want to preview locally:

```
bundle install
bundle exec jekyll serve
```

Ruby on Windows is fiddly — easiest path is the [RubyInstaller](https://rubyinstaller.org/) with the DevKit.

## Enabling GitHub Pages

In the repo on github.com: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: main / (root)**. The site will be live at `https://alex4165.github.io` within a minute or two of the first push.
