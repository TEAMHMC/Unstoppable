# HMC Unstoppable

Standalone landing page for the Health Matters Clinic Unstoppable program. ASICS Move Her Mind-inspired layout. Static HTML + assets, no build step.

## Sections

A. Hero (rotating photo carousel)
B. Mission slider
C. Intro Stories carousel
D. Stories grid + article overlay
E. Share Your Story (form posts to `volunteer.healthmatters.clinic/api/public/unstoppable-stories`)
F. Resources & Products (filterable)
G. The Report
H. Supporters
I. Footer + FAQ

## Deploy

Push to `main`. The GitHub Actions workflow at `.github/workflows/deploy.yml` publishes everything in the repo root to GitHub Pages.

1. Create the GitHub repo (e.g. `TEAMHMC/Unstoppable`)
2. Settings → Pages → Source: **GitHub Actions**
3. Push to `main` — workflow runs, page goes live at `https://teamhmc.github.io/Unstoppable/`
4. Embed in Webflow with an iframe:
   ```html
   <iframe src="https://teamhmc.github.io/Unstoppable/" style="width:100%;border:0;min-height:100vh" loading="lazy" title="HMC Unstoppable"></iframe>
   ```

## Asset paths

All assets are referenced with relative paths (`./photos/...`, `./unstoppable-logo.png`, etc.) so the page works at any subpath.
