# Overworld releases

Overworld reads live game state from RetroArch and shows it as a companion screen and OBS overlays. This repo holds its downloads.

## Install on the AYN Thor

1. Download `overworld-vX.Y.Z-android-arm64.apk` from the [latest release](../../releases/latest).
2. Open it on the Thor (from the Files app or the browser). Android asks once to let that app install apps. Allow it.
3. Open Overworld. It asks for notifications and for access to your ROMs. Both are optional.

To check the download, compare its SHA-256 with `SHA256SUMS-android.txt` on the same release.

Overworld needs Android 13 or later and an arm64 device, and a RetroArch nightly build (the Play Store build lacks network commands) with Network Commands turned on.

## Updates

Overworld checks for a new version at most once a day, when you open it. You can turn that off in Settings → Updates. When there is one, it shows the version and notes. Nothing installs until you tap Update and confirm in Android's installer.

The check downloads one file, `update-android.gdaupdate`, from this repo's latest release. It sends nothing about you or your device. Android refuses an update that is not signed by the same key as the installed app.

## Add to Obtainium

[Obtainium](https://github.com/ImranR98/Obtainium) can track this repo instead.

**[Add Overworld to Obtainium](https://apps.obtainium.imranr.dev/redirect?r=obtainium://app/%7B%22id%22%3A%22com.greatdesktopapps.overworld%22%2C%22url%22%3A%22https%3A%2F%2Fgithub.com%2FGreatDesktopApps%2Foverworld-releases%22%2C%22author%22%3A%22GreatDesktopApps%22%2C%22name%22%3A%22Overworld%22%7D)** (open this on the Thor; Obtainium shows what it will add before adding it)

Or, in Obtainium, tap **Add App** and paste:

```
https://github.com/GreatDesktopApps/overworld-releases
```
