# Adil Baadsha — Android-installable web app

## What is included
- `index.html`: your customized app
- `manifest.webmanifest`: app name, icon and standalone display settings
- `service-worker.js`: app-shell offline caching
- `icons/`: 192px and 512px app icons

## Install on Android
1. Upload the contents of this folder to an HTTPS static web host. The files must be at the site root (so `index.html` is the homepage).
2. Open the resulting HTTPS website in Chrome on your Android phone.
3. Tap Chrome's ⋮ menu and choose **Install app** or **Add to Home screen**.
4. Confirm. The installed app name is **Adil Baadsha**.

A local `file://` HTML file cannot be installed as a PWA. PWA installation requires HTTPS (or localhost for testing).

## Important data note
The app stores its progress in browser `localStorage`. The hosted version has a different browser origin from the original local file, so existing progress may not automatically transfer. Keep the original HTML and any browser data as a backup. Do not store sensitive financial or health information in this app.
