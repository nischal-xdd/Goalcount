# Ronaldo Goals Widget (Android)

This is an Android Studio source project for a home-screen widget that displays the career-goal counter from https://ronaldo.fyi/road-to-1000-goals.

## Easiest: build in the cloud (no Android Studio)
1. Create a free GitHub repo and upload this whole folder (including the hidden `.github` folder).
2. Open the **Actions** tab > **Build APK** > **Run workflow**.
3. When it finishes, download the `RonaldoGoalsWidget-apk` artifact, unzip, and install `app-debug.apk` on your Redmi.

## Or build locally
1. Install Android Studio on a computer and open this folder as a project.
2. Allow Gradle sync (requires internet to download Android Gradle Plugin and SDK components).
3. Select **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
4. Android Studio will show the APK location, usually `app/build/outputs/apk/debug/app-debug.apk`.
5. Transfer the APK to your Redmi and install it. You may need to approve installing apps from that file manager.
6. On the Redmi home screen, long-press empty space > Widgets > Ronaldo Goals Widget, then drag it onto the screen.

## Notes
- The widget starts with 981 as a fallback, based on the tracker page when this project was prepared. Tap **Refresh** to fetch the current number.
- Android limits periodic widget refreshes; this project requests 30-minute updates, plus manual refresh.
- The tracker site may change its HTML, which could require updating the parser.
- This environment did not have Gradle or the Android SDK installed, so an APK was not compiled here.
