VICE CITY HQ — V6.17 PWA EDITION

This package preserves the supplied V6.17 index.html, including its existing Supabase cloud connection, and adds installable Progressive Web App support.

FILES TO UPLOAD TO THE ROOT OF THE EXISTING GitHub Pages REPOSITORY
- index.html
- manifest.webmanifest
- sw.js
- icon-192.png
- icon-512.png

INSTALL
1. Keep your current live files and V6.16/V6.17 backups unchanged until the new version is tested.
2. Extract this ZIP.
3. Upload all five files above to the ROOT of the existing repository (the same folder as the current index.html).
4. Commit/publish and wait for GitHub Pages to finish.
5. On your Android phone, open https://jakeywesley.github.io/vice-city-hq/ in Chrome.
6. Open Chrome's three-dot menu and choose "Install app" (or "Add to Home screen", depending on Chrome's wording).
7. Launch Vice City HQ from the new home-screen icon.

WHAT THE PWA ADDITIONS DO
- Adds the app name "Vice City HQ", standalone launch mode, theme colours and app icons.
- Registers a service worker that caches the app shell and serves the cached page when offline.
- Updates the cached app shell when a newer page is successfully fetched.

IMPORTANT LIMITATIONS
- The dashboard's local data remains in browser localStorage as before.
- Supabase cloud sign-in/sync requires an internet connection.
- Spotify embeds/radio and other external services require an internet connection.
- Offline support covers the app shell; it does not guarantee every external image, embed or live countdown data source will work offline.
- The first visit must be online so the service worker can install and cache the app.
- GitHub Pages must serve the site over HTTPS (it does).

ROLLBACK
If anything behaves unexpectedly, restore your previous index.html and remove the PWA manifest/service-worker/icon files from the repository. Keep your backup ZIP.
