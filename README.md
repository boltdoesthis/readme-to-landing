# README → Landing

Free micro-tool from **Indie Agent Ship Kit** (`indieagentkit`).

Paste a README or product blurb → get a clean, single-page landing HTML you can download and host. Everything runs in the browser. No build step, no accounts, no paid APIs.

## Features

- Client-side Markdown/plain-text parsing (title, tagline, bullets, price, CTA link)
- Live preview with three themes (Ink, Paper, Mint)
- Download or copy the generated HTML
- Static files only — works on GitHub Pages, Cloudflare Pages, Netlify, or any static host
- Offline-capable after first load

## Files

| File | Role |
|------|------|
| `index.html` | App (HTML + CSS + JS in one file) |
| `README.md` | This file |

## Local preview

Open `index.html` in a browser, or serve the folder:

```bash
# Python
python3 -m http.server 8080

# Node (if you have npx)
npx --yes serve -p 8080
```

Then visit `http://localhost:8080`.

## Deploy (free)

### GitHub Pages

1. Create a public repo (e.g. `readme-to-landing`) under your anonymous brand org/user.
2. Push this folder as the repo root (or put files in `/docs` and set Pages source to `/docs`).
3. Settings → Pages → Deploy from branch → `main` / root (or `/docs`).
4. Site URL: `https://<user-or-org>.github.io/readme-to-landing/`

### Cloudflare Pages

1. Push the same repo to GitHub/GitLab.
2. Cloudflare Dashboard → Workers & Pages → Create → Connect to Git.
3. Framework preset: **None**. Build command: empty. Output directory: `/` (repo root).
4. Deploy. Optional: attach a custom domain later.

Full dual-asset publish steps: see `/workspace/DEPLOY.md` in the ship workspace (or the copy you keep with your release notes).

## License

MIT — Indie Agent Ship Kit / indieagentkit.

## Brand

Public brand only: **Indie Agent Ship Kit** / **indieagentkit**.

## Need it done for you?

Fixed-price micro-help (landing pages, launch packs, skill packs): https://boltdoesthis.github.io/indie-agent-services/
Email: boltdoesthis@gmail.com
