# Urolithin A · Discovery Dashboard

Single-page interactive dashboard (React + Tailwind via CDN) presenting a
single-ingredient case study: Discovery Flywheel and BioSeq views.

## Files
- `index.html` — the app (edit this)
- `bioseq-images.js` — large base64 image payload loaded at runtime (do not edit by hand)
- `images/` — the same figures as standalone PNGs (optional, for hosting individually)

## Run locally
Serve over HTTP (not file://) so the separate JS loads:

    python3 -m http.server 8000
    # then open http://localhost:8000

Or use the VS Code "Live Server" extension.

## Hosting
Deployed via GitHub Pages. The published URL can be embedded in Wix using an
HTML iframe element pointed at the page URL.

## Note for Claude Code
`bioseq-images.js` is ~6 MB of base64 and will blow the context window.
`.claude/settings.json` denies reading it. Don't @-mention or open it.
