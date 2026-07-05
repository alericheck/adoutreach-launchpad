# Video Ads Launchpad — Marketing Funnel Page

Static landing page for the AdOutreach Video Ads Launchpad funnel. No build step — plain HTML + JS, deployable on any static host.

## Structure

- `index.html` — the page
- `support.js` / `image-slot.js` — page runtime (required, keep next to index.html)
- `assets/` — logo + client logos
- `uploads/` — photos and screenshots used on the page

## Deploy on Cloudflare Pages

1. Push this folder to a GitHub repository (files at the repo root, not nested in a subfolder).
2. In the Cloudflare dashboard: **Workers & Pages → Create → Pages → Connect to Git** and pick the repo.
3. Build settings:
   - Framework preset: **None**
   - Build command: *(leave empty)*
   - Build output directory: `/`
4. Deploy. The site will be live at `<project>.pages.dev`; add a custom domain under the project's **Custom domains** tab.

Any push to the connected branch redeploys automatically.
