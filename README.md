# ctiolab.com

Website of CTIOLab LLC. Plain HTML and CSS, no build step.

## Structure

- `index.html`: company home page (CTIOLab logo) with a card per app
- `support.html`: support for all CTIOLab apps
- `inventory/`: the CTIOLab Inventory app section (app logo in the product bar)
  - `index.html` overview, `pricing.html`, `guide.html` (user guide and video tutorials),
    `privacy.html`, `terms.html`
  - `privacy.html` and `terms.html` are copies of the app's legal pages (tpow-inventory/public/legal). Keep them in sync.
- Future apps get their own folder, e.g. `marketplace/`, plus a card on the home page.
- `assets/`: stylesheet, logos, screenshots; `assets/docs/` holds the user guide PDF
- `vercel.json`: clean URLs, and redirects from the old addresses (/pricing, /guide, /privacy, /terms, /legal/*) to `/inventory/...`

Logos: `assets/img/ctiolab-logo.png` is the company wordmark (site header and footer).
`assets/img/inventory-logo.png` is the CTIOLab Inventory app logo (home page card and the Inventory section bar).
`assets/img/logo.png` / `logo-light.png` are the older Inventory logo, no longer used on the site.
`assets/img/marketplace-logo.png` is the CTIOLab Marketplace app logo.

Videos are embedded from YouTube; don't commit video files (GitHub rejects files over 100 MB). See `.gitignore`.

Deploy: the Vercel project `ctiolab-website` is connected to this GitHub repository, so pushing to `main` deploys www.ctiolab.com.
