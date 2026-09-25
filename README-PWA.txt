MagNervex PWA package
=====================

Deployment
- Upload all files and the icons/ folder together, preserving the folder structure.
- Serve the app over HTTPS (or localhost for development). Do not open index.html via file://.
- The first online visit installs the app-shell offline cache. Keep the service worker and assets at the same deployment path.

Install
- Android: open the site in Chrome, then use the browser menu > Install app (or Add to Home screen).
- iOS: open the site in Safari, tap Share > Add to Home Screen.

Updates
- After publishing a release, change CACHE_NAME in service-worker.js (for example, magnervex-pwa-v2). The activation handler removes older MagNervex caches; revisit online to install the updated cache.
