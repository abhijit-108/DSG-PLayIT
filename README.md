# 🎬 DSG PlayIT

<p align="center">
  <img src="https://raw.githubusercontent.com/abhijit-108/DSG-PLayIT/main/logo.png" alt="DSG PlayIT Logo" width="120" height="120" />
</p>

<p align="center">
  <strong>A modern, high-performance MX Player Pro alternative for Android built with Jetpack Compose & AndroidX Media3 ExoPlayer.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Version-v2.0.1-9D4EDD?style=for-the-badge" alt="Version" />
  <img src="https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Platform" />
  <img src="https://img.shields.io/badge/Kotlin-2.3.20-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white" alt="Kotlin" />
  <img src="https://img.shields.io/badge/Compose-BOM_2026.03-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white" alt="Compose" />
  <img src="https://img.shields.io/badge/Media3-ExoPlayer_1.5.1-FF007F?style=for-the-badge" alt="Media3" />
</p>

---

## 🌟 Overview

**DSG PlayIT** is an advanced, hardware-accelerated offline video player designed for Android. Combining the intuitive gesture workflow of **MX Player Pro** with a sleek neon dark aesthetic, DSG PlayIT offers seamless media playback, multi-track audio selection, integrated subtitle rendering, and native Picture-in-Picture (PiP).

---

## ✨ Features

### 📂 Smart Folder-Based Media Library
- **Automatic Device Scanning**: Leverages Android's `MediaStore` to aggregate all video files on internal and SD card storage.
- **Clean Path Display**: Strips redundant root storage prefixes (`/storage/emulated/0/`) to show intuitive relative folder paths (e.g. `Download/Quick Share`, `Movies/DSG Records`).
- **Live Search & Quick Filter**: Instant keyword search to locate folders within milliseconds.
- **Dynamic Sorting**: Sort video folders by **Video Count**, **Folder Name**, or **Date Modified**.
- **Detailed Video Metadata**: Video cards show file size, container format, and file creation date formatted as `Size • Format • dd/MM/yy  hh:mm a` (e.g. `369.7 MB • MP4 • 03/09/26  09:16 pm`).

### 🎛️ MX Player Pro Signature Gestures
- **Vertical Volume Gesture**: Swipe up/down on the **right side** of the screen to adjust volume with a vertical rising neon pill slider, adaptive volume icons, and percentage display.
- **Vertical Brightness Gesture**: Swipe up/down on the **left side** of the screen to smoothly regulate screen brightness.
- **Horizontal Seek Scrubber**: Swipe horizontally across the screen to quickly scrub forward/backward with instant time offset preview (`+00:15`, `-00:30`).
- **Double-Tap Quick Seek**: Double-tap on left or right edges to skip 10 seconds with ripple animations.
- **Auto-Hide Controls**: Dynamic overlay that fades out after 4 seconds of inactivity during playback.

### 🚀 Ultra-Slim Video Seek Bar
- **Precision 3dp Profile**: Replaced bulky default sliders with a slim 3.dp track that expands subtly to 5.dp during scrubbing.
- **Buffer Progress Indicator**: Real-time visual track showing buffered chunks in soft white.
- **Smooth Scrubbing**: Generous 28.dp touch hit-area with tap-to-seek and 120fps fluid scrubbing.
- **Glowing Thumb**: Refined neon circular thumb indicator.

### 🎧 Multi-Track Audio & Subtitle Engine
- **Sanitized Metadata**: Clean ISO-639 language tag resolution (e.g., *English, Hindi, Japanese*), eliminating corrupted raw placeholders (`\`, `...`, `und`).
- **Audio Codec & Channels**: Displays audio format specifics (*AAC • Stereo*, *AC-3 • 5.1 Surround*, *Mono*).
- **Subtitle Switching**: Built-in support for embedded and external subtitles (SRT, ASS, SSA, VTT).
- **Compact Overlay Pills**: Header pills display shortened action labels: `[ 🔤 Sub: OFF ]`, `[ 🎵 Audio 1 ]`, `[ 📐 Landscape ]`, `[ ⏱️ 1.0x ]`.

### ⚡ Hardware Acceleration & PiP
- **Hardware-Accelerated Codecs**: Supported hardware decoding via `MediaCodec` for H.264 (AVC), H.265 (HEVC), VP9, AV1, MPEG-4, TS, MKV, MP4, and WebM.
- **Picture-in-Picture (PiP)**: Smooth automatic transition to a floating PiP window when leaving the app.
- **Aspect Ratio Modes**: Cycle between **Fit to Screen**, **Stretch / Fill**, **Zoom / Crop**, **16:9**, and **4:3**.
- **Playback Speed**: Adjust speed dynamically from `0.5x` to `2.0x`.
- **Playback State Persistence**: Automatically remembers and resumes the last played position per video.

---

## 🛠️ Tech Stack & Architecture

- **Language**: Kotlin 2.3.20
- **UI Framework**: Jetpack Compose (Material 3, Material Icons Extended)
- **Media Engine**: AndroidX Media3 ExoPlayer 1.5.1
- **Image Loading**: Coil Compose 2.7.0 (Video Frame Decoder)
- **Architecture**: Modern Android MVVM (Model-View-ViewModel) + StateFlow + Coroutines
- **Target OS**: Android 8.0 (API 26) through Android 16 (API 36)

---

## 📥 Download & Installation

1. Go to the **[Releases](https://github.com/abhijit-108/DSG-PLayIT/releases)** tab on GitHub.
2. Download the latest **`DSG-PlayIT-v2.0.1.apk`**.
3. Open the downloaded `.apk` file on your Android device.
4. When prompted, enable **"Install from unknown sources"** for your browser or file manager.
5. Launch **DSG PlayIT** and grant media permission to immediately browse and play your offline video collection.

---

## 🔒 Permissions

DSG PlayIT requires the following permissions to index and stream local media files:

| Permission | Purpose |
| :--- | :--- |
| `READ_MEDIA_VIDEO` | Access video files on Android 13+ (API 33+) |
| `READ_EXTERNAL_STORAGE` | Access video files on Android 12 and below |

---

## 📋 Changelog

### `v 2.0.1`
- **Slimline Video Seek Bar**: Custom 3.dp seekbar with buffer caching progress and glowing micro-thumb.
- **Vertical Gesture Controls**: Upgraded volume and brightness swipe controls to vertical edge-aligned capsule sliders.
- **Shortened Overlay Pills**: Compact `[ Sub: OFF/ON ]` and `[ Audio 1 ]` action badges.
- **Home Screen Branding**: Added bold purple neon `v 2.0.1` version badge below the app title.

### `v 2.0.0`
- **Sanitized Track Metadata**: Fixed corrupted ISO tag rendering (`\` and `...` artifacts).
- **Picture-in-Picture (PiP)**: Added native backgrounding PiP support.
- **Brand Identity**: Integrated purple crystal neon app logo and icon assets.
- **Package Migration**: Standardized application ID to `com.delsgade.playit`.

### `v 1.1.0`
- **Metadata Formatting**: Added file size, format, and creation date (`dd/MM/yy  hh:mm a`).
- **Path Sanitization**: Stripped root storage paths to begin cleanly after `emulated/0/`.

### `v 1.0.0`
- **Initial Release**: Core Jetpack Compose video player engine with MediaStore folder indexing and Media3 ExoPlayer integration.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
