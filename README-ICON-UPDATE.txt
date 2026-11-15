VICE CITY HQ — ICON UPDATE

Upload these four files to the ROOT of your existing GitHub repository:
- icon-192.png
- icon-512.png
- sw.js
- README-ICON-UPDATE.txt (optional; this is just the instruction file)

Replace the two existing icon PNGs and replace sw.js. Do not delete or replace
index.html or manifest.webmanifest.

The service-worker cache has been bumped to v2 so the updated icon assets can
be fetched. After GitHub Pages finishes publishing, open the site in Chrome,
refresh it, then close and reopen the installed app.

Android may keep the old launcher icon cached. If it does, remove the home-screen
app shortcut/install and install Vice City HQ again from Chrome. Your website
data is stored separately; do not clear site storage.
