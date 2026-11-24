# Harun Khan: academic website

A Jekyll site that GitHub Pages builds automatically. It has an academic home page and a blog with **Academic** and **Personal** posts.

## Writing a post

1. Create `_posts/YYYY-MM-DD-short-title.md`, e.g. `_posts/2026-12-01-verified-bitblasting.md`.
2. Start it with front matter:

   ```yaml
   ---
   title: "Verified bit-blasting in Lean"
   subtitle: Optional one-line summary shown in post lists.
   categories: academic   # or: personal
   math: true             # only if the post uses LaTeX ($...$ and $$...$$)
   ---
   ```
3. Write the body in Markdown, then commit and push. The post appears on `/blog/`, under its category, on the home page's "Recent Writing" list and in the RSS feed (`/feed.xml`).

`_drafts/example-academic-post.md` is a template showing math, code and formatting. Files in `_drafts/` are never published. Put images in `assets/` and reference them as `![alt]({{ '/assets/pic.png' | relative_url }})`.

## Layout

| Path | What it is |
| --- | --- |
| `index.html` | Home page (bio, news, publications, CV sections) |
| `_posts/` | Published blog posts |
| `_drafts/` | Unpublished drafts |
| `blog/` | Blog index plus `academic/` and `personal/` filters |
| `_layouts/`, `_includes/` | Page templates |
| `style.css` | All styles, with automatic light and dark mode |

## Preview locally

```sh
bundle install
bundle exec jekyll serve --drafts   # http://localhost:4000/
```

## Deploy

In the repo, go to **Settings → Pages**, choose **Deploy from a branch**, then pick the branch and `/ (root)`.

**Custom domain:** buy the domain, then add a `CNAME` file containing it (e.g. `harunkhan.org`). In `_config.yml`, set `url: "https://harunkhan.org"` and `baseurl: ""`. Then point DNS at GitHub Pages and enter the domain under Settings → Pages.
