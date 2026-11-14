# Overworld releases

Overworld reads live game state from RetroArch and shows it as a companion screen and OBS overlays. This repo holds its downloads.

## Install on the AYN Thor

1. On the Thor, open [greatdesk.app/overworld-android](https://greatdesk.app/overworld-android) and tap the download link. It always points at the newest version. (Every version is also on the [releases page](../../releases), under tags that start with `android-v`.)
2. Open it on the Thor (from the Files app or the browser). Android asks once to let that app install apps. Allow it.
3. Open Overworld. It asks for notifications and for access to your ROMs. Both are optional.

To check the download, compare its SHA-256 with `SHA256SUMS-android.txt` on the same release.

Overworld needs Android 13 or later and an arm64 device, and a RetroArch nightly build (the Play Store build lacks network commands) with Network Commands turned on.

## Updates

What changed in each version: [android/CHANGELOG.md](android/CHANGELOG.md).

Overworld checks for a new version at most once a day, when you open it. You can turn that off in Settings → Updates. When there is one, it shows the version and notes. Nothing installs until you tap Update and confirm in Android's installer.

The check downloads one file, [android/update-android.gdaupdate](android/update-android.gdaupdate), from this repo. It sends nothing about you or your device. Android refuses an update that is not signed by the same key as the installed app.

## Add to Obtainium

[Obtainium](https://github.com/ImranR98/Obtainium) can keep Overworld up to date.

**[Add Overworld to Obtainium](https://apps.obtainium.imranr.dev/redirect?r=obtainium://app/%7B%22id%22%3A%22com.greatdesktopapps.overworld%22%2C%22url%22%3A%22https%3A%2F%2Fgreatdesk.app%2Foverworld-android%22%2C%22author%22%3A%22GreatDesktopApps%22%2C%22name%22%3A%22Overworld%22%2C%22additionalSettings%22%3A%22%7B%5C%22versionExtractionRegEx%5C%22%3A%5C%22overworld-v%28%5C%5C%5C%5Cd%2B%5C%5C%5C%5C.%5C%5C%5C%5Cd%2B%5C%5C%5C%5C.%5C%5C%5C%5Cd%2B%29-android%5C%22%2C%5C%22matchGroupToUse%5C%22%3A%5C%221%5C%22%2C%5C%22appAuthor%5C%22%3A%5C%22GreatDesktopApps%5C%22%7D%22%7D)** (open this on the Thor; Obtainium shows what it will add before adding it)

Or, in Obtainium, tap **Add App** and paste:

```
https://greatdesk.app/overworld-android
```

and set **Version extraction regular expression** to `overworld-v(\d+\.\d+\.\d+)-android`, with match group `1`. Obtainium then shows real version numbers.

Obtainium names the author after the page's host, greatdesk.app. To show GreatDesktopApps instead, open Overworld in Obtainium, tap the pencil button (**Additional options**) and set **Author** to `GreatDesktopApps`. The Add Overworld to Obtainium link above sets this for you.

If you already track this GitHub repo in Obtainium, that keeps working. There's no need to switch.
