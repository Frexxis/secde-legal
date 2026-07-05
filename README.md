# secde-legal (GitHub Pages)

This repository hosts Secde app legal documents via GitHub Pages.

Published paths (project site):

- `/secde-legal/privacy/`
- `/secde-legal/terms/`
- `/secde-legal/support/`
- `/secde-legal/tr/privacy/` and `/secde-legal/tr/terms/`
- `/secde-legal/ar/privacy/` and `/secde-legal/ar/terms/`
- `/secde-legal/de/privacy/` and `/secde-legal/de/terms/`
- `/secde-legal/fr/privacy/` and `/secde-legal/fr/terms/`

## Deploy

1. Push to `main`.
2. In GitHub: `Settings -> Pages -> Build and deployment -> Source: GitHub Actions`.

The workflow deploys `public/`.

## Update legal text

Do not edit `public/` by hand.

Canonical legal text lives in the main app repo under `legal/canonical/`.

From the main repo root, regenerate both bundled app assets and this site with:

```bash
node scripts/generate_legal_outputs.mjs
```

Then commit the generated changes and redeploy by pushing to `main`.
