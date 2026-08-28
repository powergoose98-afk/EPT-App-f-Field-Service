# Test Bench — Field Testing Reference

A mobile-first PWA reference for field service technicians: NETA-scope electrical
equipment acceptance/maintenance test procedures, a troubleshooting-pitfalls library
by test instrument, tappable inspection checklists, and a device-local SATSU content
import. Offline-capable, installable to the home screen.

## Deploy to GitHub Pages
1. Create a repo and upload the entire contents of this folder to the repo root
   (index.html must be at the top level, not inside a subfolder).
2. Settings → Pages → Source: Deploy from branch → `main` / root → Save.
3. Wait 1–2 min, open the Pages URL on a phone, then Share → Add to Home Screen.

## Files
- `index.html` — the entire app: content, styling, and logic in one file.
- `sw.js` — service worker (offline cache). Bump the `CACHE` version string
  when you publish changes so installed phones pull the update.
- `manifest.json`, `icons/` — PWA install metadata and home-screen icons.
- `images/` — optional product photos named by equipment ID (see images/README.txt);
  a photo overrides the built-in line-art illustration automatically.
- `satsu-template.json` — starter file for SATSU content; import via the in-app
  gear icon → Import. Content is stored only on the device, never in this repo.

## Editing content
All testing and troubleshooting content lives in the `EQ` and `TS` objects inside
the `<script>` in index.html. Standards references are in the `REFS` array.

## Important
This is a reference aid. Acceptance values and table data must be verified against
your licensed NETA ATS/MTS edition, the manufacturer's instruction book, and Eaton
SATSU. NETA renumbered sections in ATS-2021; ATS-2025 supersedes it — treat the
in-app reference numbers as approximate.
