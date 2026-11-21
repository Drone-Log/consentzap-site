# consentzap.app

Static site for ConsentZap. No build step, no external resources, no cookies, no analytics.

- `index.html` — landing page
- `privacy.html` — privacy policy (also needed for App Store / AMO listings)
- `style.css` — shared styles (light + dark)
- `favicon.svg`
- `CNAME` — custom domain for GitHub Pages

## Publish (GitHub Pages)

1. Repository → Settings → Pages → Source: *Deploy from a branch*, branch `main`, folder `/`.
2. Custom domain: `consentzap.app` (read from `CNAME`), then tick **Enforce HTTPS** once the certificate is issued.
3. DNS at the registrar for `consentzap.app`:
   - `A` records → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `AAAA` records → `2606:50c0:8000::153`, `2606:50c0:8001::153`, `2606:50c0:8002::153`, `2606:50c0:8003::153`
   - optional `CNAME` for `www` → `<github-user>.github.io`

`.app` domains are HTTPS-only (HSTS preloaded), so the site works only after GitHub has issued the certificate.
