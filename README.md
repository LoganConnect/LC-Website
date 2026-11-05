# Logan Connect website

One-page static site for Logan Connect, an independent nonprofit community organisation based at Park Ridge Baptist Church, Logan, Queensland. Plain HTML, CSS and JavaScript; no build step. All paths are relative, so it works at a GitHub Pages project URL and at a custom domain.

## Status: preliminary

The reference page (https://prbc.org.au/logan-connect/) could not be accessed when this was built, so no content was invented. Items marked `[... to be supplied]` and elements with `data-placeholder` need replacing.

Source material needed:
- Official wording for Who We Are, Our Purpose, Neighbour in Need, Community Breakfast and Get Involved
- Breakfast day/time/location and any programme details
- Contact email, phone, address, ABN/legal details
- Logo, photographs and graphics (place in `assets/`)

## Files
`index.html`, `style.css`, `script.js`, `assets/`, `.nojekyll` (disables Jekyll processing).

## Local preview
`python3 -m http.server 8000`, then open http://localhost:8000

## Deploy to GitHub Pages
1. Merge to the default branch.
2. Repository **Settings → Pages**: Source "Deploy from a branch", branch `main`, folder `/ (root)`.
3. The site appears at `https://<user>.github.io/logan-connect/`.

### Custom domain (loganconnect.com.au)
1. In Settings → Pages, set Custom domain to `loganconnect.com.au` and enable Enforce HTTPS.
2. At the DNS provider, add `A` records for the apex to GitHub Pages IPs (185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153) and a `CNAME` for `www` to `<user>.github.io`.
3. Optionally add a `CNAME` file containing `loganconnect.com.au` to the repo root.
