<p align="center">
  <img src="assets/icon.png" width="128" alt="Device Hub for Android icon">
</p>

<h1 align="center">Device Hub for Android</h1>

<p align="center"><b>Browse, copy and mirror your Android phones on your Mac — in one window.</b><br>
Native macOS app. USB or Wi‑Fi. No account, no cloud, no data collection.</p>

<p align="center">
  <a href="https://github.com/hoangvunam/Device-Hub-for-Android/releases/latest"><img alt="Download for macOS" src="https://img.shields.io/badge/Download-GitHub%20Releases-2ea44f?style=for-the-badge&logo=apple&logoColor=white"></a>
  <img alt="Mac App Store: coming soon" src="https://img.shields.io/badge/Mac%20App%20Store-coming%20soon-lightgrey?style=for-the-badge&logo=appstore&logoColor=white">
</p>

<p align="center"><a href="README.vi.md">🇻🇳 Tiếng Việt</a></p>

<p align="center">
  <img src="assets/files-dark.png" alt="File browser with image preview (dark)">
</p>

## Features

**Files**
- Several phones at once, with a sidebar of favorite folders (Downloads, Camera, Pictures, Movies, Music, Documents), internal storage and app folders
- Browse, rename, create folders, delete, show hidden files, back/forward/up history
- Instant preview of images and videos in the inspector, with size, permissions and path
- Drag files from Finder onto the window (or onto the phone screen), use the **Import** button (⇧⌘I) or paste from Finder with ⌘V to copy them to the phone; download to your Mac with one click
- With nothing selected, the inspector shows the open folder: item count, size and an Import button

**Transfers**
- Fast direct transfers with a queue, live progress, cancel, and conflict handling (ask / keep both / replace / skip)
- Two phones side by side in a split view
- Photo & video import: scans DCIM / Pictures / Movies and copies only new items into `YYYY/YYYY-MM` folders, never overwriting

**Connections**
- **Wi‑Fi pairing** with a QR code or a six-digit code (Android 11+); USB and Wi‑Fi links to the same phone appear as one device, and the app offers to switch if one link drops
- **No USB debugging needed for files:** set the phone to *File transfer* (MTP) or *Transfer photos* (PTP) and browse, copy, rename, delete and preview right away. Turn on USB debugging when you want mirroring and apps — the app switches over and keeps your folder
- **Android emulators:** start and shut down Android Studio emulators from the sidebar, mirror them, and change the fold state of foldable models

**Screen mirroring & control**
- Live phone screen next to your files (or in its own window), with touch, keyboard, scroll and Vietnamese (Telex) text input
- Two-way clipboard, device audio, rotate, screenshot and screen recording
- Back / Home / Recents / volume / power buttons

**Apps & device**
- Manage apps: list, install APK, uninstall
- Battery level and storage at a glance

**Made for the Mac**
- SwiftUI, Liquid Glass on macOS 26, Light / Dark, interface in 20 languages
- Bundled `adb` and `scrcpy-server` — nothing else to install

| Mirror (light) | Mirror (dark) |
|---|---|
| <img src="assets/mirror-light.png" alt="Mirror, light mode"> | <img src="assets/mirror-dark.png" alt="Mirror, dark mode"> |

> Screenshots use sample photos from [Unsplash](https://unsplash.com).

## Requirements

- macOS 14 Sonoma or later (Apple silicon and Intel)
- An Android phone and a data-capable USB cable. *File transfer* mode is enough for files; screen mirroring and app management need **USB debugging**
- Wi‑Fi pairing needs Android 11+ with the phone and Mac on the same network
- Audio capture needs Android 11+; tested on Android 12 and 17

## Install

1. Download the latest `Device-Hub-for-Android-x.y.z.dmg` from [Releases](https://github.com/hoangvunam/Device-Hub-for-Android/releases/latest), open it and drag **Device Hub for Android** to Applications. The app is signed with Developer ID and notarized by Apple.
2. Files only: connect the phone, unlock it and choose **File transfer** in the USB notification — done. For mirroring and apps, also turn on USB debugging: **Settings → About phone →** tap *Build number* 7 times, then **Settings → System → Developer options → USB debugging**.
3. Connect the phone by USB and tap **Allow** on the "Allow USB debugging?" prompt (tick *Always allow*).

**Mac App Store version:** it runs inside the App Sandbox with its own adb key, so you must tap **Allow USB debugging** on the phone once more the first time you connect.

## FAQ

**The phone shows "Unauthorized" or does not appear.** Unlock the phone, replug the cable, and accept the USB debugging prompt. Try *Revoke USB debugging authorizations* in Developer options if the prompt never appears. Make sure the cable supports data and the USB mode is not "charging only".

**Do I need to install adb or scrcpy?** No. Both are bundled. If another `adb` of a different version is already running, adb restarts its server once — this is normal.

**Does it work over Wi‑Fi?** Yes. Choose *Connect over Wi‑Fi…* and pair with a QR code or a six-digit code from *Developer options → Wireless debugging* (Android 11+). Files never leave your local network.

**Do I have to turn on USB debugging?** Not for files. In *File transfer* mode the app uses the standard MTP protocol through macOS. Screen mirroring and app management need USB debugging.

**Is my data sent anywhere?** No. Everything goes directly between your Mac and your phone over USB or your local network. There are no accounts, analytics or network calls to our servers.

**File names with accents or emoji?** Supported (Unicode is preserved end to end).

**Why does the phone screen not show for some apps?** Apps that block screen capture (e.g. banking apps using `FLAG_SECURE`) appear black — this is enforced by Android.

## Privacy

Device Hub for Android collects no data. See the [Privacy Policy](PRIVACY.md) and [Terms of Use](TERMS.md).

## Third-party software

- [scrcpy](https://github.com/Genymobile/scrcpy) server (v3.1) — © Genymobile, Apache License 2.0
- Android SDK Platform-Tools (`adb`) — © The Android Open Source Project, Apache License 2.0; downloaded from Google's official distribution

Full notices are in the app (*Settings → About → Open Third-Party Notices*).

## Support

Email [namhv.cntt@gmail.com](mailto:namhv.cntt@gmail.com) or visit the [support page](SUPPORT.md).

---

This repository only hosts release downloads and documentation; it does not contain the source code.
© 2026 Hoàng Vũ Nam. Android is a trademark of Google LLC. Device Hub for Android is an independent product and is not affiliated with or endorsed by Google.
