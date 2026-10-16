# BodyTrack Atlas

Interactive body atlas — click a body part to see which datasets apply and track findings over time.

Live site (after GitHub Pages enable): `https://<your-username>.github.io/bodyatlas/`

## Run locally

Just open `index.html` in a browser, or serve it:

```bash
npx serve .
# or
python3 -m http.server 8000
```

## Deploy to GitHub Pages

This repo is a static site (`index.html` only). Pages is enabled automatically on push via Actions, or enable manually:

1. Push to GitHub
2. Repo → Settings → Pages → Deploy from branch → `main` / `/ (root)`
3. Visit the Pages URL

## Structure

- `index.html` — entire app (UI + CSS + JS + dataset list)
- `atlas.html` — original file, same as `index.html`

## Add datasets

Edit the `D.push(...)` list in `index.html`, or use “Add your own dataset” in the UI (saved to localStorage).
