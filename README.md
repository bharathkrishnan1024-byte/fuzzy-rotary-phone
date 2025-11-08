# NEET PG Accountability Tracker (PWA-ready)

This repository contains a lightweight single-file tracker for NEET PG / INI-CET preparation, updated to be PWA-ready for easy installation on mobile phones.

## Files included
- `index.html` - Main app (was final.html) — ready to be uploaded to a static host.
- `manifest.json` - PWA manifest for "Add to Home Screen".
- `service-worker.js` - Minimal service worker to cache the app shell.
- `icon-192.png`, `icon-512.png` - Simple app icons.
- `LICENSE` - MIT License.
- `README.md` - This file.

## How to deploy (fast)
1. Rename or ensure `index.html` exists (already done).
2. Push these files to a public GitHub repository.
3. Enable GitHub Pages for the repo, or drag & drop the files to Netlify. Both will serve over HTTPS.
4. Open the site on a mobile browser. Use "Add to Home Screen" (or the browser prompt) to install it like an app.

## Notes & recommendations
- The original local ChatGPT/localhost integration has been commented out/removed for public hosting to avoid runtime errors. If you want a hosted chat feature, add a proper remote API and secure the endpoint.
- For best offline experience, expand `service-worker.js` caching rules to include additional assets and handle versioning.
- If you want a custom domain, configure it via GitHub Pages / Netlify settings.
