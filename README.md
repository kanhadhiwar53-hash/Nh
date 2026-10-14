# NHSeries Android App

Android application project. The GitHub Actions workflow is configured to build a debug APK.

## Build APK with GitHub Actions
1. Open the **Actions** tab.
2. Select **Android APK**.
3. Click **Run workflow** (or push a commit to `main`).
4. Open the completed run and download the `NHSeries-debug-apk` artifact.

The workflow uses JDK 17 and Gradle 8.2. The Android project must be committed under `NHSeries/` or the repository root.

## Local build
From the Android project directory, run:
```bash
gradle assembleDebug
```

APK output: `app/build/outputs/apk/debug/app-debug.apk`.
