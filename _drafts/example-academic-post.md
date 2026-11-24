---
title: "Example post: how to write one"
subtitle: A template showing everything a post can do. Files in _drafts/ are never published.
categories: academic   # academic or personal
math: true             # turn on LaTeX rendering for this post
---

To publish a post, create a file in `_posts/` named `YYYY-MM-DD-short-title.md`
with front matter like the block at the top of this file. Set `categories` to
`academic` or `personal`.

## Math

Inline math like $a^2 + b^2 = c^2$ works, and so do display equations:

$$
\sum_{k=1}^{n} F_k^2 = F_n F_{n+1}
$$

## Code

```lean
theorem add_comm' (a b : Nat) : a + b = b + a := by
  omega
```

```python
def fib(n):
    a, b = 0, 1
    for _ in range(n):
        a, b = b, a + b
    return a
```

## Everything else

> Block quotes, **bold**, *italics*, [links](https://lean-lang.org/), lists
> and images (put them in an `assets/` folder) all work as normal Markdown.

1. First
2. Second
