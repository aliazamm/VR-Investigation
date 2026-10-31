# VR Investigation Android

A basic Android WebView wrapper for an existing Google Apps Script web app.

## Before building

1. Open `app/src/main/java/com/vr/investigation/MainActivity.kt`.
2. Replace `PASTE_YOUR_DEPLOYMENT_ID_HERE` in `startUrl` with your deployed Apps Script Web App URL.
3. Replace `app/src/main/res/drawable/ic_logo.xml` if you want a different launcher logo. Keep it as a valid Android vector drawable, or update the manifest icon path to match your replacement.

## Build APK on GitHub

1. Upload the contents of this project to the root of a GitHub repository (not the containing folder).
2. Keep the repository private if it contains private project code.
3. Open the **Actions** tab.
4. Select **Build VR Investigation APK**.
5. Click **Run workflow**. A push to the `main` branch also starts a build.
6. When the run succeeds, open it and download the `VR-Investigation-APK` artifact.
7. Extract the downloaded ZIP to get `app-debug.apk`.

## Notes

- This creates a debug APK for testing, not a Play Store release.
- The app requires an internet connection.
- Google sign-in may be blocked in embedded WebViews by Google's security policy. If your web app relies on Google account sign-in, test the login flow; a supported external-browser sign-in flow may be needed.
- Do not put passwords, API secrets, or private credentials in this repository.
