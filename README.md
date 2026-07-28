# Dhruv Surana — Portfolio

Personal portfolio for **Dhruv Surana** — Business Analytics & AI student at UT Dallas, focused on
**Data Analytics, Business Intelligence, Analytics Engineering, and Product Management**.

Live, static, dependency-free website built with plain **HTML, CSS, and JavaScript** (no build step).

## Structure

```
.
├── index.html            # The entire site (HTML + inline CSS + inline JS)
├── favicon.svg           # Brand favicon
├── site.webmanifest      # PWA manifest
├── robots.txt            # Crawler rules + sitemap reference
├── sitemap.xml           # Single-page sitemap
├── vercel.json           # Vercel caching + security headers (used only on Vercel)
├── .nojekyll             # Disable Jekyll on GitHub Pages
├── .github/workflows/
│   └── deploy.yml        # Auto-deploy to GitHub Pages on every push to main
├── assets/               # Resume PDF + Open Graph image
├── images/               # Photos, logos, project thumbnails (WebP)
└── icons/tools/          # Local tool/technology SVG logos
```

## Local preview

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deployment

This repo is configured to auto-deploy to **GitHub Pages** via GitHub Actions
(`.github/workflows/deploy.yml`). Any push to `main` republishes the site.

The site is also 100% compatible with **Vercel** and **Netlify** with zero changes
(`vercel.json` is included for optimal caching/headers on Vercel).

### Update workflow

```
edit index.html  →  git commit  →  git push  →  site redeploys automatically
```

## Custom domain

To use a domain like `dhruvsurana.com`, add a `CNAME` file (GitHub Pages) or add the
domain in the platform dashboard (Vercel/Netlify), then point DNS at the platform.
See the deployment notes for details.
