# secde-legal (GitHub Pages)

This repository hosts Secde app legal documents via GitHub Pages.

Published paths (expected by the app/store metadata):

- `/privacy/`
- `/terms/`
- `/support/`
- `/tr/privacy/` and `/tr/terms/`
- `/ar/privacy/` and `/ar/terms/`
- `/de/privacy/` and `/de/terms/`
- `/fr/privacy/` and `/fr/terms/`

## Deploy

1. Push to `main`.
2. In GitHub: `Settings -> Pages -> Build and deployment -> Source: GitHub Actions`.

The workflow deploys `public/`.

## Update legal text

Edit the relevant HTML page under `public/` and redeploy by pushing to `main`.
