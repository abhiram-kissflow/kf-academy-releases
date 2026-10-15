# Kissflow Academy

A desktop app for learning to build on Kissflow: lessons, quick checks, hands-on exercises in your own training tenant with a coach beside you, a final assessment and a certificate.

## Download

| Platform | Download | Notes |
|---|---|---|
| **macOS** (Apple Silicon and Intel) | [Kissflow-Academy-macos-universal.dmg](https://github.com/abhiram-kissflow/kf-academy-releases/releases/latest/download/Kissflow-Academy-macos-universal.dmg) | One download for both chip types |
| **Windows** 10 and 11 (64-bit) | [Kissflow-Academy-windows-x64-setup.exe](https://github.com/abhiram-kissflow/kf-academy-releases/releases/latest/download/Kissflow-Academy-windows-x64-setup.exe) | Installs for the current user |
| **Linux** (x86_64) | [Kissflow-Academy-linux-x86_64.AppImage](https://github.com/abhiram-kissflow/kf-academy-releases/releases/latest/download/Kissflow-Academy-linux-x86_64.AppImage) | Runs on most distributions; updates itself |
| **Linux** (Debian, Ubuntu) | [Kissflow-Academy-linux-amd64.deb](https://github.com/abhiram-kissflow/kf-academy-releases/releases/latest/download/Kissflow-Academy-linux-amd64.deb) | Installs system-wide; does not update itself |
| **Android** 7 and later | [Kissflow-Academy-android-arm64.apk](https://github.com/abhiram-kissflow/kf-academy-releases/releases/latest/download/Kissflow-Academy-android-arm64.apk) | Almost every phone and tablet from the last decade (25 MB) |
| **Android**, older 32-bit phones | [Kissflow-Academy-android-armv7.apk](https://github.com/abhiram-kissflow/kf-academy-releases/releases/latest/download/Kissflow-Academy-android-armv7.apk) | If the one above says "App not installed" (19 MB) |
| **Android**, Chromebooks and emulators | [Kissflow-Academy-android-x86_64.apk](https://github.com/abhiram-kissflow/kf-academy-releases/releases/latest/download/Kissflow-Academy-android-x86_64.apk) | Intel and AMD devices (24 MB) |
| **Android**, not sure | [Kissflow-Academy-android.apk](https://github.com/abhiram-kissflow/kf-academy-releases/releases/latest/download/Kissflow-Academy-android.apk) | Works on every Android device, bigger download (64 MB) |

Every link always points at the newest version. Older versions and release notes are on the [Releases](https://github.com/abhiram-kissflow/kf-academy-releases/releases) page.

## Install

The app is not yet signed with an Apple or Microsoft developer certificate, so the first launch shows a warning. This is expected.

**macOS.** Open the `.dmg` and drag Kissflow Academy into Applications. On first launch macOS says it cannot verify the developer: open **System Settings › Privacy & Security**, scroll down, and click **Open Anyway**. You only do this once.

**Windows.** Run the installer. If SmartScreen shows "Windows protected your PC", click **More info › Run anyway**. The installer fetches Microsoft Edge WebView2 if your PC does not already have it.

**Linux AppImage.** Make it executable, then run it:

```bash
chmod +x Kissflow-Academy-linux-x86_64.AppImage
./Kissflow-Academy-linux-x86_64.AppImage
```

On Ubuntu 24.04 and later, AppImages need FUSE 2 first: `sudo apt install libfuse2t64`.

**Linux .deb.**

```bash
sudo apt install ./Kissflow-Academy-linux-amd64.deb
```

The `.deb` does not update itself. To get a new version, download and install the new `.deb`, or use the AppImage instead.

**Android.** Download the `.apk` on your phone and open it. Android asks you to allow installs from your browser or file manager the first time: turn on **Allow from this source**, go back, and tap **Install**. Play Protect may warn that the app is from an unknown developer; tap **Install anyway**.

On Android, coaching sessions keep the course and Kiko in the app, and **Kissflow ↗** in the session rail opens your training account in the browser. Switch between the two, or use split screen on a tablet. Android versions do not update themselves. To update, install the newer `.apk` over the old one; your progress is kept. All four Android files are the same app, so you can switch between them the same way.

## Updates

The macOS, Windows and AppImage versions check for updates when they start and every 30 minutes. When one is available, the button in the app's header says **Update to x.y.z**: click it, then **Restart to update**. Updates are cryptographically signed and verified before they install.

## Your data

Your progress, answers and chats stay on your computer or phone. Nothing is sent to Kissflow or to the course authors. The only network traffic is to the AI provider you choose in Settings, your own Kissflow training tenant, and this page for updates.

## About this repository

This repository only hosts the installers and the update manifest (`latest.json`). The source code is private.
