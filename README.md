# ctiolab.com

Static website for CTIOLab LLC. Plain HTML and CSS, no build step.

- `index.html`, `pricing.html`, `support.html`: marketing pages
- `guide.html`: user guide page; the PDF is `assets/docs/ctiolab-ims-user-guide.pdf`
- `privacy.html`, `terms.html`: copies of the app's legal pages (tpow-inventory/public/legal). Keep them in sync when either changes.
- `assets/`: stylesheet, logo, screenshots
- `vercel.json`: clean URLs (/pricing instead of /pricing.html)

Videos are embedded from YouTube; don't commit video files (GitHub rejects files over 100 MB). See `.gitignore`.

Deploy: the Vercel project `ctiolab-website` is connected to this GitHub repository, so pushing to `main` deploys www.ctiolab.com.
