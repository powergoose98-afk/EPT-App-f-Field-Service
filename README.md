# Test Bench — Field Testing Reference PWA

NETA-scope electrical equipment testing reference for field service technicians.
Reference-only (v1). Offline-capable, installable to home screen.

## Deploy to GitHub Pages
1. Create a repo (e.g. `test-bench`), push these files to the root of `main`.
2. Repo Settings → Pages → Source: Deploy from branch → `main` / root.
3. Open the Pages URL on your phone → Share → Add to Home Screen.

## Structure
- `index.html` — entire app + all reference content (edit the `EQ` object to change content)
- `sw.js` — service worker (bump `CACHE` version string when you publish content changes)
- `manifest.json`, `icons/` — PWA install metadata

## Important
Acceptance values/table data must be verified against your licensed NETA ATS/MTS
edition, the manufacturer's IB, and Eaton SATSU. SATSU sections are stubbed
pending company documents.
