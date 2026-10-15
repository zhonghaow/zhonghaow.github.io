# Zhonghao Wang — personal website

A simple, responsive personal website based on `CV_20260924.pdf`, with `head.jpg` as the portrait. Plain HTML and CSS; no build step or dependencies.

## Preview

Open `index.html` directly in a browser, or run from this folder:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Then open <http://localhost:8000>.

## Edit

- `index.html`: introduction, links, experience, research, and education.
- `styles.css`: typography, spacing, and mobile layout.
- `head.jpg`: original portrait.
- `CV_20260924.pdf`: source CV, kept for reference and not linked on the website.
- `favicon.svg`: browser icon.
- `sitemap.xml`: the site's page list for search engines; update `lastmod` when `index.html` changes.
- `robots.txt`: allows all crawlers and points them to the sitemap.
- `CNAME`: the GitHub Pages custom domain, `zhonghaowang.com`.
- `.nojekyll`: tells GitHub Pages to serve this static site without Jekyll processing.

## Publish

The site is hosted by GitHub Pages from the root of the `main` branch in [zhonghaow/zhonghaow.github.io](https://github.com/zhonghaow/zhonghaow.github.io).

To publish updates, commit `index.html`, `styles.css`, `favicon.svg`, `head.jpg`, `sitemap.xml`, `robots.txt`, `.nojekyll`, and `CNAME` to that repository. GitHub Pages deploys changes automatically. No build step, server-side code, or environment variables are required.

The custom domain is `zhonghaowang.com`, managed through Squarespace Domains. Its website DNS records should be:

| Type | Host | Value |
| --- | --- | --- |
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `zhonghaow.github.io` |

In the repository's **Settings → Pages**, set the custom domain to `zhonghaowang.com` and enable **Enforce HTTPS** once GitHub has issued its certificate. Keep domain email records and nameservers intact when updating website records.

The site uses system fonts and has no analytics, cookies, or external JavaScript.
