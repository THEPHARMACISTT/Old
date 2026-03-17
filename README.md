# Tracker Made Easy — PWA

A fully offline-capable Progressive Web App for shift tracking.

## Files

```
tracker-pwa/
├── index.html       ← Main app (open this in browser)
├── manifest.json    ← PWA metadata
├── sw.js            ← Service Worker (offline support)
├── icon-192.png     ← App icon
├── icon-512.png     ← App icon (large)
└── README.md
```

## How to install / use

### Option A — Local file (quickest)
Just open `index.html` in Chrome/Safari on your phone. Works immediately.
*Note: Service Worker won't activate on `file://` URLs. For full PWA install, use Option B.*

### Option B — Host it (recommended for install prompt)

**Free hosting options:**

1. **Netlify Drop** (zero-signup, instant):
   - Go to https://app.netlify.com/drop
   - Drag the entire `tracker-pwa` folder into the browser
   - Get a live URL instantly — share it, open on phone, tap "Add to Home Screen"

2. **GitHub Pages**:
   - Create a repo, upload these files
   - Enable Pages in repo Settings → Pages → Deploy from branch
   - Visit `https://yourusername.github.io/reponame`

3. **Vercel / Cloudflare Pages**: Upload folder, get instant URL

### Installing on phone

**iOS (Safari)**:
1. Open your hosted URL in Safari
2. Tap the Share button (□↑)
3. Tap "Add to Home Screen"
4. Done — appears as an app icon!

**Android (Chrome)**:
1. Open your hosted URL in Chrome
2. Tap the ⋮ menu → "Add to Home Screen"
   or wait for the install banner to appear
3. Done!

## Data storage

All data is saved in **localStorage** — it stays on your device, no account needed.
Use Settings → Export to back up your data as JSON.

## Changes from Claude.ai version

- Storage: `window.storage` (Claude API) → `localStorage` (standard browser)
- Added: Service Worker for offline use
- Added: Web App Manifest for installability
- Added: PWA icons
- Everything else is identical
