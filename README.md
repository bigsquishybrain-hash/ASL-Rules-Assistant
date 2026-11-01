# ASL Rules Assistant

Offline-capable web app (PWA): ASL Sequence of Play tracker, IFT / Morale / Rally / Close Combat engine, and a searchable rulebook digest with chart tables.

## Files
- `index.html` : the entire app (rule data embedded, about 3 MB)
- `manifest.webmanifest`, `icon-*.png`, `apple-touch-icon.png` : install metadata
- `sw.js` : service worker for offline use

## Publish with GitHub Pages
1. Put all files in the root of a repo (or a `/docs` folder).
2. Repo Settings > Pages > Deploy from a branch > pick the branch and folder > Save.
3. Open `https://<your-user>.github.io/<repo>/` once while online.

## Install
- **iPad / iPhone (Safari):** Share > Add to Home Screen.
- **Android (Chrome):** menu > Install app (or Add to Home screen).

After the first load it runs offline. Sequence of Play state is saved on the device.

## Updating
Replace `index.html`, then change `VERSION` in `sw.js` (for example `asl-rules-v2`) and commit. Devices pick up the new copy the next time they open the app online.
