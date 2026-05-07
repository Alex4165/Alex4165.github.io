---
title: Example post
date: 2026-05-07
math: true
---

This is an example post. The filename is `_posts/2026-05-07-example-post.md` — the `YYYY-MM-DD-slug.md` format is required by Jekyll. Front matter at the top sets the title, date, and (when needed) `math: true` to load KaTeX on the page.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

## A second-level heading

You can write **bold**, *italics*, `inline code`, and [links](https://example.com). Footnotes work too[^1].

[^1]: Like this one.

### A third-level heading

Lists:

1. First item
2. Second item
3. Third item

- Bullet
- Bullet
- Bullet

A blockquote:

> Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.

A code block:

```python
def fib(n):
    a, b = 0, 1
    for _ in range(n):
        a, b = b, a + b
    return a
```

A small table:

| Symbol | Meaning      |
|--------|--------------|
| $n$    | sample size  |
| $\mu$  | mean         |
| $\sigma$ | std. dev.  |

## Math

Inline math uses backslash-paren: \\( e^{i\pi} + 1 = 0 \\).
Does \(e=mc^2\) not work?
Display math uses double dollars or backslash-brackets:

$$
\int_{-\infty}^{\infty} e^{-x^2}\,dx = \sqrt{\pi}
$$

Aligned equations:

$$
\begin{aligned}
\nabla \cdot \mathbf{E} &= \frac{\rho}{\varepsilon_0} \\
\nabla \cdot \mathbf{B} &= 0 \\
\nabla \times \mathbf{E} &= -\frac{\partial \mathbf{B}}{\partial t} \\
\nabla \times \mathbf{B} &= \mu_0 \mathbf{J} + \mu_0 \varepsilon_0 \frac{\partial \mathbf{E}}{\partial t}
\end{aligned}
$$

A note on inline math: use `\(...\)` rather than `$...$` so plain dollar signs in prose (e.g. "it cost $5") don't get treated as math delimiters.

---

To add a new post, drop a Markdown file into `_posts/` named `YYYY-MM-DD-your-slug.md`, set `math: true` in the front matter if you need formulas, and write. That's it.
