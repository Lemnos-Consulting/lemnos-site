# lemnos.io

Source for the [Lemnos Consulting](https://lemnos.io) marketing site.

## Structure

- `index.html` — single-page site (HTML + inline CSS + inline JS, no build step)
- `CNAME` — custom domain config for GitHub Pages

## Deployment

GitHub Pages serves from the `main` branch. Pushing to `main` deploys automatically.

## Contact form

The contact form POSTs JSON to an n8n webhook at `https://lemnos.app.n8n.cloud/webhook/lead-intake`. The webhook workflow must be published in n8n for the form to work.

## Local preview

Open `index.html` directly in a browser — no server required.
