MY PERSONAL TOOL KIT — PWA PACKAGE

Files:
- index.html: application
- manifest.webmanifest: install metadata
- sw.js: same-origin offline app-shell cache
- icons/: install icons

INSTALL / HOSTING
1. Upload the contents of this folder together to a static web host with HTTPS (for example, your own hosting account).
2. Open the HTTPS URL in a supported browser.
3. Use the browser's Install App / Add to Home Screen command.

For local testing, serve this folder from http://localhost (not by double-clicking index.html). Service workers generally require HTTPS or localhost. The service worker caches the app shell and same-origin files only; third-party resources such as Google Fonts are not cached. Test all app tools and backup/restore after deployment. Browser storage remains tied to the browser/device and is not automatically synchronized between devices.

SECURITY NOTE
A standalone PWA is not a secure identity boundary. Client-side password checks and embedded code can be inspected or modified by someone with access to the files/device. Do not treat PWA packaging as server-side access control.
