Remote-100 four-variant Android build

Legacy: Android 2.2+, minSdk 8, targetSdk 28
Lollipop: Android 5.0+, minSdk 21, targetSdk 28
Oreo: Android 8.0+, minSdk 26, targetSdk 28
Modern: Android 12+, minSdk 31, targetSdk 35

Build with JDK 17, Gradle 8.9, Android SDK platform 35:
    gradle assembleDebug

GitHub Actions: upload this project to a GitHub repository, then run
Actions > Build Remote-100 APK variants > Run workflow.
Download the artifact containing all four debug APKs.

NOTE: Builds have not been executed here: Android SDK and Gradle are not
installed in this environment. Modern Android permission flow was added,
but runtime behavior and Bluetooth hardware connectivity remain untested.
Google Play may impose additional requirements. Android 15/16 may restrict
installing the old legacy-targeted APKs; use the modern variant there.
