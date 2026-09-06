# 🎬 DSG PlayIT

<p align="center">
  <img src="https://raw.githubusercontent.com/abhijit-108/DSG-PLayIT/main/app_logo.png" alt="DSG PlayIT Logo" width="100" height="100" />
</p>

<p align="center">
  <strong>Fast, minimal, hardware-accelerated offline video player for Android with MX Player Pro-style gestures. Built with Jetpack Compose & AndroidX Media3 ExoPlayer.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Version-v2.1.6-9D4EDD?style=for-the-badge" alt="Version" />
  <img src="https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Platform" />
  <img src="https://img.shields.io/badge/Kotlin-2.3.20-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white" alt="Kotlin" />
  <img src="https://img.shields.io/badge/Compose-Material_3-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white" alt="Compose" />
  <img src="https://img.shields.io/badge/Media3-ExoPlayer-FF007F?style=for-the-badge" alt="Media3" />
</p>

---

## ✨ Features

- **Intuitive Gestures**: Vertical swipe for Volume (right) & Brightness (left), horizontal swipe seek, double-tap to skip, and hold for 2x speed.
- **Hardware-Accelerated Playback**: Powered by AndroidX Media3 ExoPlayer supporting H.264, H.265 (HEVC), VP9, AV1, MKV, MP4, WebM, and more.
- **Audio & Subtitle Switching**: Multi-track audio selection with clean language labels and embedded/external subtitle support.
- **Modern Glassmorphic Controls**: Clean translucent player controls, vibrant gradient play button, and 3dp slimline seek bar.
- **Aspect Ratio Modes**: Quick toggle between Fit to Screen, Crop / Zoom, and Stretch with top-right on-screen HUD indicator and saved preferences.
- **Folder Media Library**: Auto-scans local storage, groups videos into folders, and displays file size chip badges with enlarged thumbnails.
- **In-App GitHub Updater**: Built-in update checker with changelog display and live APK download progress.
- **Picture-in-Picture (PiP)**: Native floating mini-player when leaving the app.

---

## 🛠️ Tech Stack

| Component | Technology |
| :--- | :--- |
| **Language** | Kotlin 2.3.20 |
| **UI Framework** | Jetpack Compose (Material 3) |
| **Media Engine** | AndroidX Media3 ExoPlayer 1.5.1 |
| **Image Loading** | Coil Compose (Video Frame Decoder) |
| **Architecture** | MVVM + StateFlow + Coroutines |
| **Compatibility** | Android 8.0 (API 26) - Android 16 (API 36) |

---

## 📥 Download

Download the latest APK directly from the repository:

- 📦 **[Download latest app-debug.apk](https://raw.githubusercontent.com/abhijit-108/DSG-PLayIT/main/app-debug.apk)**
- 🏷️ **[GitHub Releases](https://github.com/abhijit-108/DSG-PLayIT/releases)**

---

## 📋 Changelog

### `v 2.1.6`
- **Video Card Redesign**: File size in a dedicated chip badge, larger thumbnails, and high-contrast date & time on a separate line.
- **Aspect Ratio HUD Indicator**: Top-right on-screen popup showing applied mode (*Fit to Screen, Crop / Zoom, Stretch*) with saved preferences.
- **Streamlined Player Controls**: Removed redundant 10s skip buttons in favor of double-tap gestures; widened button spacing with glassmorphic borders.
- **Compact Video Info Dialog**: 2-column specs grid fitting all details without scrolling, and clean relative file path (starts after `emulated/0/`).

### `v 2.1.5`
- **Settings & Preferences**: Minimal grouped settings for Playback, Gestures, and AMOLED Pure Black mode.
- **In-App GitHub Updater**: Direct update checking, changelog preview popup with dismissible 'Later' option, and live APK download progress.
- **Clean UI**: Removed search buttons for a distraction-free home and folder screen.

### `v 2.0.1`
- **Slimline Seek Bar**: Precision 3dp seekbar with live buffer caching indicator and glowing micro-thumb.
- **Vertical Gesture HUDs**: Capsule volume and brightness sliders aligned to the screen edges.

### `v 2.0.0`
- **Track Sanitization**: Cleaned audio and subtitle language tags.
- **Picture-in-Picture (PiP)**: Background floating player support.
- **Brand Identity**: Updated app logo and purple neon theme.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
