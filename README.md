# BodyTrack Atlas — cross-species anatomy index

Pick an organism, then an anatomical region, to get the right open imaging datasets — with in-browser analysis and longitudinal tracking.

Live site: `https://harshini-suresha.github.io/bodyatlas/`

## Organisms (9) · 500+ datasets

Human · Mouse · Rat · Macaque · Marmoset · Pig · Zebrafish · Fruit fly · C. elegans — each with species-specific regions, verified sources, mirrors, pipelines and a built-in image/CSV analyser. Human keeps the full body figure, 3D models and lesion-timeline demo; other species get embedded microCT/CT Sketchfab models where free scientific ones exist, plus authoritative viewers and free STL/model links.

The human index aggregates 400+ entries from the OpenMedLab Awesome-Medical-Dataset catalog and the TCIA collections archive, plus curated model-organism resources. Every link is HTTP-verified; use Export CSV/JSON in the Collection overview card to take the filtered list with you.

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
