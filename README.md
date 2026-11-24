# Harun Khan: academic website

A static personal site: plain HTML and CSS with no build step.

- `index.html`: all page content
- `style.css`: styles, with automatic light and dark mode
- `cv.pdf`: the CV linked from the page

## Preview locally

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy with GitHub Pages

In the repo, go to **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, then pick the branch and `/ (root)`.
The site will be served at `https://harunk-dev.github.io/website/`. To serve it at `https://harunk-dev.github.io/` instead, rename the repo to `harunk-dev.github.io`.
