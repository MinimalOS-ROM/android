# Minimal OS 1.0

**Minimal OS** is a lightweight, distraction-free custom Android 12.1 (LineageOS 19.1-based) ROM designed specifically for dumbphones and flip phones such as the **Cat S22 Flip**.

## Features

- **Clean, Minimal UI**: Customized SystemUI, launcher (Trebuchet), and dialer tailored for small screens and physical keypads.
- **Built on LineageOS 19.1**: Inherits stability, security, and device compatibility from Android 12.1 / LineageOS 19.1.
- **Distraction-Free Experience**: Focused on essential communication and utility without bloat.

## Getting Started

### 1. Initialize the Repository

```bash
repo init -u https://github.com/MinimalOS-ROM/android.git -b minimal-1.0
```

### 2. Sync the Source

```bash
repo sync -c -j$(nproc) --force-sync --no-clone-bundle --no-tags
```

### 3. Build

Set up your build environment and build for your target device (e.g., Cat S22 Flip):

```bash
source build/envsetup.sh
breakfast <device_codename>
brunch <device_codename>
```

## Modified Repositories

- [`android_frameworks_base`](https://github.com/MinimalOS-ROM/android_frameworks_base) — SystemUI / QS tile customizations
- [`android_packages_apps_Dialer`](https://github.com/MinimalOS-ROM/android_packages_apps_Dialer) — Dumbphone-friendly dialer & monochrome theme
- [`android_packages_apps_Trebuchet`](https://github.com/MinimalOS-ROM/android_packages_apps_Trebuchet) — Minimal launcher & app drawer
