# CHERA Android

This is an offline Android wrapper for the original CHERA interface. The original HTML/CSS/JavaScript is bundled at `app/src/main/assets/index.html`; it is not hosted or loaded from a website.

## Build
Run `gradle assembleDebug` from this directory with JDK 17 and Android SDK platform 35 installed. The APK is created at `app/build/outputs/apk/debug/app-debug.apk`.

The GitHub Actions workflow `.github/workflows/android.yml` builds and uploads the APK as an artifact when manually dispatched or when Android project files change.

## Notes
- The UI source is bundled locally and kept unchanged from the repository's original `index.html`.
- The Android file chooser grants access to user-selected audio/video files.
- Background playback and lock-screen media controls need a dedicated native media playback integration and device testing; this initial APK build does not claim those features are complete.
