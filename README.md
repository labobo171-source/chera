# CHERA

A Persian RTL, mobile-first music player web app with a neon glass interface.

## Current features
- Local audio/video file selection and folder selection where supported by the browser
- Playlist, favorites, shuffle, repeat-one and repeat-all
- Web Audio processing with 10-band EQ, soft bass, treble boost and output gain
- Animated circular spectrum visualizer
- Five themes: Neon, Cyberpunk, Galaxy, Matrix and Gold
- Driving mode
- Media Session actions where supported
- PWA manifest and offline app-shell service worker

## Run locally
Serve this directory over HTTPS or localhost. Opening `index.html` directly with `file://` limits PWA and some browser APIs.

## Browser limitations
A website cannot silently scan all phone storage. The user must select files or a folder, and folder selection support varies by browser. Local object URLs are temporary, so files generally need to be selected again after a reload. Background playback and lock-screen controls depend on browser and operating-system support. Full Android background service integration requires a native Android wrapper.

## Development
This is the initial static HTML/CSS/JavaScript PWA prototype. Test on Android Chrome and desktop browsers before production deployment.


## Enable GitHub Pages
The repository's Actions integration currently cannot enable Pages automatically. In the repository, open **Settings → Pages → Build and deployment**, set **Source** to **GitHub Actions**, and save. The deployment workflow will then publish the site after a push to `main`.

