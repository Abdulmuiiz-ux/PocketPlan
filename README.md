# PocketPlan MVP

PocketPlan is a responsive personal budget and expense tracker built with HTML, CSS and JavaScript. It is packaged as a Progressive Web App (PWA), so it can be published as a website and installed from a supported browser.

## Features
- Set/update a budget
- Add expenses with categories and dates
- See spending and remaining budget
- Search and delete expenses
- Export expenses to CSV
- Saves data in browser `localStorage`
- Offline app shell after first successful online visit
- Installable PWA manifest with 192px, 512px and maskable icons

## Run locally
For a quick preview, open `index.html`. To test service-worker and installation behaviour, serve this folder over localhost:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`. PWA installation requires HTTPS when deployed (localhost is treated as secure for development).

## Publish free with GitHub Pages
1. Create a GitHub repository and upload the **contents** of this folder (`index.html`, `manifest.json`, `sw.js`, and the PNG icons).
2. In the repository, open **Settings → Pages**. Choose deployment from the main branch and root folder, then save.
3. Wait for GitHub Pages to provide a public HTTPS URL.
4. Open that URL on your phone. On Android, use the browser menu and choose **Install app** or **Add to Home screen**. On iPhone/iPad in Safari, tap **Share → Add to Home Screen**.

Alternative static hosts include Netlify or Cloudflare Pages. Upload the files in this folder and use the HTTPS URL they provide.

## Important limitations
- This is an installable web app (PWA), not yet a native app submitted to Google Play or Apple's App Store. Store distribution usually requires a wrapper/build process, developer accounts, and store review.
- Data is stored only in the current browser/device. Clearing browser data may erase it, and data does not sync between devices.
- No user accounts, cloud sync, bank integrations, or shared multi-user storage.
- Do not store sensitive financial details in this prototype.
