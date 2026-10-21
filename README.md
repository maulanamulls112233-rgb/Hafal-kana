# Hiragana Arena Android APK

This project packages the HTML game in `app/src/main/assets/index.html` into a native Android APK using a WebView. GitHub Actions builds a debug APK and exposes it as a downloadable workflow artifact.

## Build APK on GitHub
1. Upload the **contents** of this folder to the root of your GitHub repository (keep the `.github/workflows/build-apk.yml` file).
2. Open the repository's **Actions** tab.
3. Select **Build Hiragana Arena APK** and press **Run workflow**, or push a commit to `main`/`master`.
4. When the workflow finishes with a green check, open that run and download **HiraganaArena-APK** from Artifacts. Extract the ZIP to get `HiraganaArena.apk`.

## Notes
- This produces a debug APK for testing/installing directly on Android, not a Play Store release-signed APK.
- User data saved in browser local storage remains on that device/app installation; it is not automatically synced across devices.
- Review and test login, audio, and game flows on your target devices before sharing broadly.
