# DroidSuite - from the comfort of the terminal.

**Note:** This tool requires ADB debugging enabled on your Android device. Some features (e.g., global uninstalls or full device searches) require root access.

## Features

### Device Information
- Generate a comprehensive system report including:
  - Brand, model 
  - Android version, SDK 
  - Serial, build, security patch, kernel
  - Arch, supported archs
  - Root
  - Uptime
  - Storage usage
  - Memory info 
  - Screen resolution
  - Wi-Fi name, IP address
  - CPU, GPU

### App Management
- Install APKs (single files or from folder).
- Uninstall apps (with root support for global removal).
- Enable/disable apps (user or system-wide with root).
- Clear app data and cache (per app or just cache for all apps).

### File Management
- Pull/push files and folders between device and PC.
- Delete files/folders on the device.
- Search for files or folders

### Custom Settings
- TV Tweaks: Optimize animations, caches, and UI for better performance on Android TV devices (Android 9+).
- DNS Settings: Set private DNS providers (Cloudflare, Mullvad, AdGuard, etc.) or custom hostnames.
- Capture screenshots.
- Check for system updates.

### Developer Tools
- View, save, or clear logcat logs.
- Open an interactive ADB shell.
- Execute custom ADB commands.

## Requirements
- **Operating System:** Linux.
- **Dependencies:** 
  - `android-tools if arch and android-tools-adb if debian`

- **Device Setup:**

- How to Enable Developer Options on your Device

Go to Settings.

Tap About phone.

Tap Build number (usually under "Software information") seven times rapidly.

You will see the message "You are now a developer!"
Developer options is now available in the main Settings menu.


- USB cable,IP Adress of the device.
- **Optional:** Root access on the device for advanced features.

## Installation
1. Download the Script:
   ```
   wget https://raw.githubusercontent.com/RonKamonohashi/DroidSuite/refs/heads/main/DroidSuite
   curl -O https://raw.githubusercontent.com/RonKamonohashi/DroidSuite/refs/heads/main/DroidSuite
   ```
2. Make the script executable:
   ```
   chmod +x DroidSuite
   ```

The script will check for `android-tools if arch and android-tools-adb if debian` and promt you the correct install command.

## Usage
1. Launch the script: `./DroidSuite`.
2. Select a connection method.
3. Navigate through the interactive menus using numbers.
4. Follow on-screen prompts for each feature.

**Tips:**
- For root features, ensure your device is rooted (e.g., via Magisk).
- Use cautiously: Some operations (e.g., uninstalls, tweaks) are irreversible without backups.
- If ADB fails, ensure no port conflicts and accept the debugging prompt on your device.

## Acknowledgments
- Thanks to the ADB Devs.
- Inspired by the FOSS community .


