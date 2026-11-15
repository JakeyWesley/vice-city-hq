VICE CITY HQ — V6.18 PREVIEW

This is a separate preview package. It does not replace your live V6.17/V6.17-era app.

WHAT'S NEW
- New Weather at HQ panel on the Home screen.
- Weather is requested only when you tap “Check weather”.
- Your browser asks permission before sharing location.
- Current temperature, feels-like temperature, conditions and wind are shown.
- If permission is denied or the service is unavailable, the rest of HQ continues working.

PRIVACY
- The app does not save your coordinates.
- Coordinates are sent to Open-Meteo only to retrieve the forecast.
- No location request is made automatically.

PRESERVED
- Existing tabs, event planner, countdowns, inventory, Friday Club, cat gallery,
  radio/playlist integration, local save data and cloud-sync code are retained.
- Existing PWA manifest, service worker and icons are carried forward.

TESTING / INSTALLATION
1. Extract all files into one folder.
2. Test by hosting the folder over HTTPS (for example, a separate GitHub Pages
   branch or temporary repository). Geolocation generally will not work from
   a plain file:// open.
3. Do not overwrite your current live site until you've tested the preview.
4. If you later publish it to the same PWA URL, close the installed app and
   refresh/reopen after the service worker updates.

This is a preview build; the existing sports countdown data and other app
features have not been replaced with live third-party sports feeds in this build.
