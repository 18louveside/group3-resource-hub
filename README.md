# Group 3 Resource Hub

A lightweight, mobile-friendly, installable website for the Group 3 Bioethics Advocacy Campaign.

## Files
- `index.html` — the website
- `sw.js` — saves the site shell for offline access after the first successful online visit
- `manifest.webmanifest` — installable web app details
- `icon.svg` — app icon

## Important offline limitation
A website cannot be opened from a public link for the very first time without any connection. Open it once while online; the service worker then caches the page shell. After that, the page can reopen offline on supported browsers. The external source links still require internet.

## Publish free with GitHub Pages
1. Sign in to GitHub and create a **public** repository, for example `group3-resource-hub`.
2. Upload all four website files from this folder to the repository's top level.
3. In the repository, open **Settings → Pages**.
4. Under Build and deployment, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
5. Wait for GitHub Pages to publish. Share the resulting `https://...github.io/.../` link.
6. Open the link once while online on each device/browser that needs offline access. On supported browsers, use the browser menu or the page's Install button to add it to the home screen.

## Sharing offline
If someone has no internet at all and has never opened the website, send them the ZIP while they have access to Bluetooth, USB, or another local file-sharing method. They can open `index.html` from the extracted folder; the page content works, but installable/offline caching requires a secure hosted site (HTTPS) or local development server.

No analytics, external fonts, images, or libraries are loaded by this site.
