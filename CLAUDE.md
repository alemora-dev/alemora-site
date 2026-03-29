# Claude Context — alemora-site (Portfolio)

## What this is

Portfolio site for Alejandro Mora — AI engineer public identity.
Live at: https://alemora.me

## Stack

- **Framework:** Astro (static output)
- **Styles:** Tailwind CSS v4 — use `@import "tailwindcss"` in CSS, NOT the v3 directives
- **Hosting:** Cloudflare Pages (auto-deploy on push to `main`)
- **Repo:** `alemora-dev/alemora-site` on GitHub

## Key files

- `src/pages/index.astro` — main page (single page site)
- `src/layouts/Layout.astro` — HTML shell, imports global CSS
- `src/styles/global.css` — Tailwind import only
- `public/` — static assets

## Deploy

Push to `main` → Cloudflare Pages builds and deploys automatically.
Build command: `npm run build` | Output: `dist/`

## Design

- Dark theme: background `#0a0a0a`, text `#e8e8e8`
- Accent color: `#4ade80` (green)
- Font: system-ui
- Sections: Nav → Hero → Projects → About/Stack → Footer

## Brand context

- Do NOT reference `alemora.dev` — taken by someone else
- Do NOT reference `alejandromora.com` — another person entirely
- Tone: direct, technical, no LinkedIn fluff

## Projects

All 6 Colombia Open Data projects are live:

| App | URL | Stack |
|-----|-----|-------|
| Lupa Pública | lupa.alemora.me | Vanilla JS |
| Mi Barrio en Cifras | barrio.alemora.me | Vanilla JS |
| Respirar | respirar.alemora.me | Vite + Leaflet |
| Mercado Justo | mercado.alemora.me | Vite + Leaflet |
| Cine y Letras | cine.alemora.me | Vite + Leaflet |
| GeoChomp | geochomp.alemora.me | Vanilla JS |

To promote a project to live: add to `projects` array in `src/pages/index.astro` with subdomain URL.
To show in-progress: add `labProjects` array and split the grid (see git history for reference).
