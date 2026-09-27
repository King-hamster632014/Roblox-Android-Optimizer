# Roblox Android Optimizer

This repository contains a simple Roblox performance configuration and installation links for Android tools that may help you apply it correctly.

## What is included

- `ClientAppSettings.json` — Roblox settings for lower visual load and better performance
- `Cx Install Link.txt` — link to install Cx File Explorer
- `Shuziku install` — link to install Shizuku

## Purpose

This project is meant to help improve Roblox performance on Android devices by adjusting client settings and making it easier to access the app folder where these settings are stored.

## Important notes

- Back up your current Roblox settings before modifying anything.
- This is intended for Android devices and may not work the same way on every Roblox version.
- Settings and menu names can vary by Android version and device manufacturer.
- If something does not work, restore the original file.
- Only grant Shizuku access to apps you trust.

## Instructions

### 1. Enable Developer Options

1. Open **Settings** on your Android device.
2. Open **About phone** or **About device**. On some devices, this is under **System**.
3. Find **Build number**.
4. Tap **Build number** seven times. Enter your lock-screen PIN, password, or pattern if prompted.
5. Return to Settings and open **System > Developer options**, or search Settings for **Developer options**.
6. Turn on **Developer options** if it is not already enabled.

### 2. Install and set up Shizuku on your device

1. Open the file named **Shuziku install** in this repository.
2. Follow the provided link to install the official Shizuku app.
3. Open Shizuku and choose **Start via Wireless debugging** if your device supports Android 11 or newer.
4. In **Settings > Developer options**, enable **Wireless debugging**.
5. Tap **Wireless debugging**, then choose **Pair device with pairing code**.
6. In Shizuku, tap the pairing option and enter the Wi-Fi pairing code shown by Android. Keep the Shizuku pairing screen open while entering the code if required.
7. Return to Shizuku and tap **Start** under wireless debugging. The Shizuku service should show that it is running.
8. If your device does not support wireless debugging, follow Shizuku's in-app instructions for the ADB method using a computer and USB debugging:
   - Enable **USB debugging** in **Developer options**.
   - Connect the device to the computer with a USB cable.
   - Accept the **Allow USB debugging?** authorization prompt on the phone.
   - Complete the ADB setup described in Shizuku.
9. In Shizuku, check that the service is running before opening Cx File Explorer. Shizuku may need to be started again after every device restart.

> **Note:** The exact menu names and Shizuku setup options may differ between Samsung, Xiaomi, Motorola, Pixel, and other Android devices. Use the instructions displayed in the Shizuku app for your specific device.

### 3. Install Cx File Explorer

1. Open **Cx Install Link.txt** in this repository.
2. Follow the link to install Cx File Explorer from the provided source.
3. Launch Cx File Explorer and grant the requested file-access permissions.

### 4. Locate the Roblox settings file

1. Open Cx File Explorer and use its Shizuku or elevated-access option if it provides one.
2. Navigate to the Roblox app data folder, usually similar to:

   `/data/data/com.roblox.client/`

3. Look for `ClientAppSettings.json`, commonly inside a Roblox `files` folder. The exact location may vary by Roblox version.

### 5. Replace the settings file

1. Back up the existing `ClientAppSettings.json` file before changing it.
2. Open the current file in Cx File Explorer.
3. Replace its contents with the contents of this repository's `ClientAppSettings.json`.
4. If the file does not exist, create it in the correct Roblox folder.
5. Save the file and confirm that it remains valid JSON.

### 6. Restart Roblox

1. Fully close Roblox, including removing it from recent apps.
2. Reopen Roblox and check whether performance and visuals have improved.

### 7. Adjust if needed

- If the game is still too heavy or does not work correctly, restore your backup.
- Keep the original settings file so you can revert the changes at any time.

## Recommended use

- Best for lower-end Android devices
- Useful for smoother gameplay and reduced lag
- Use only if you are comfortable editing app settings files

## Troubleshooting

- **Shizuku is not running:** Start it again from the Shizuku app. Wireless debugging services may stop after a restart.
- **Pairing fails:** Make sure Wi-Fi is enabled, the phone and pairing process are on the same network, and use a new pairing code.
- **The Roblox folder cannot be accessed:** Confirm that Shizuku is running and that Cx File Explorer supports Shizuku access.
- **Settings do not take effect:** Fully restart Roblox and verify that the file was saved in the correct folder with valid JSON syntax.
- **Performance gets worse:** Restore the original `ClientAppSettings.json` file.

## Final reminder

This repository is a small optimization helper, not a full app. Use it carefully and always keep a backup of your original Roblox settings before making changes.
