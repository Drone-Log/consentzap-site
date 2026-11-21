# consentzap.app

Website for **ConsentZap** — a browser extension for Safari and Firefox that rejects cookie-consent banners through each site's own consent tool, checks the refusal was saved, and blocks known trackers.

**Live:** https://consentzap.app

The site practises what the extension preaches: a static page with no build step, no cookies, no analytics, no external fonts or scripts.

## Files

| File | Purpose |
|---|---|
| `index.html` | Landing page |
| `privacy.html` | Privacy policy (also used for App Store / addons.mozilla.org listings) |
| `style.css` | Shared styles, light and dark |
| `favicon.svg` | Icon |
| `robots.txt` | Allows all crawlers, points to the sitemap |
| `sitemap.xml` | Page list for search engines |
| `llms.txt` | Plain-text summary for AI assistants |
| `index.md`, `privacy.md` | Markdown versions of the pages for agents (`<link rel="alternate" type="text/markdown">`); update them when the HTML text changes |
| `.nojekyll` | Serve `.md` files as-is (no Jekyll conversion) |
| `og-image.png` | Social share image (1200×630); source in `og/og.html` |
| `CNAME` | Custom domain for GitHub Pages |

## Local preview

Open `index.html` in a browser — there is nothing to build.

## Hosting

- **GitHub Pages:** branch `main`, folder `/`, custom domain `consentzap.app`, HTTPS enforced.
- **DNS:** Cloudflare, all records **DNS only** (grey cloud). Proxying would stop GitHub from issuing the HTTPS certificate, and `.app` domains only work over HTTPS.
  - `A` `@` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
  - `AAAA` `@` → `2606:50c0:8000::153`, `2606:50c0:8001::153`, `2606:50c0:8002::153`, `2606:50c0:8003::153`
  - `CNAME` `www` → `drone-log.github.io`

## Credits

The extension uses consent rules from [DuckDuckGo autoconsent](https://github.com/duckduckgo/autoconsent) (MPL-2.0) and the [Disconnect](https://disconnect.me/trackerprotection) tracker list (CC BY-NC-SA 4.0).

## License

Site code and content: [MIT](LICENSE).
