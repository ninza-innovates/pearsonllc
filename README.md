# Pearson LLC

Static marketing site for [Pearson LLC](https://pearsonllc.pro), a tech talent staffing company. The homepage is titled “Connecting Americans with Global Tech Talent”: it describes connecting US clients with international developers for affordable tech work.

This repository is the published site. There is no application server, package manifest, or build step checked in. Pages are plain HTML that share `style.css` and a prebuilt `bundle.js`.

## What’s in the repo

| Path | What it is |
| --- | --- |
| `index.html` | Homepage |
| `signin.html` | Sign-in page |
| `signup.html` | Sign-up page |
| `dashboard.html` | Dashboard page |
| `blog-grid.html` | Blog listing |
| `blog-single.html` | Single blog post |
| `404.html` | Not-found page |
| `style.css` | Site stylesheet |
| `bundle.js` | Prebuilt client script (Alpine.js, loaded with `defer` on each page) |
| `images/` | Logos, photos, icons, and other static assets |
| `favicon.ico` | Favicon |
| `CNAME` | GitHub Pages custom domain (`pearsonllc.pro`) |

Sign-in, sign-up, and dashboard are static HTML pages in this repo, not a separate backend.

## View it locally

Open `index.html` in a browser, or serve the repo root with any static file server. For example:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080/`. Other pages are linked from the site or can be opened directly (`signin.html`, `signup.html`, `dashboard.html`, `blog-grid.html`, `blog-single.html`).

## Custom domain (GitHub Pages)

`CNAME` contains a single line, `pearsonllc.pro`. On GitHub Pages, a root `CNAME` file sets the custom domain for the site. The live site is the files in this repository; nothing here needs to be compiled before publishing.
