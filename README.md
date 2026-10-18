# EditRoom for Android

EditRoom video editor packaged with Capacitor. The app itself is `www/index.html`.

## Build the APK with Android Studio
1. Install Node 20+, Android Studio and JDK 21.
2. In this folder run:
   npm install
   npx cap add android
   npx cap sync android
   npx cap open android
3. In Android Studio press Run to install on a phone or emulator,
   or use Build > Build APK(s).

## Build the APK without Android Studio
Push this folder to a GitHub repository. The workflow in
.github/workflows/android.yml builds a debug APK on every push.
Download it from the run's Artifacts section and install it on your phone
(allow "install unknown apps" when asked).

## Notes
- Export records in real time and produces a WebM file. After export, tap
  "Save or share video" to open the Android share sheet.
- Fonts load from Google Fonts when online and fall back to system fonts offline.
- After editing www/index.html run `npx cap sync android` again.
