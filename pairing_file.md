## Pairing Guide

idevice_pair allows us to create a pairing file for programs like StikDebug to talk to your device remotely. This pairing file is device-specific and required to use StikDebug, otherwise StikDebug will not function correctly. Caution: this pairing file can and will expire randomly, requiring you to remake it.

---

First, set a passcode on your device, sideload an app with the `get-task-allow` entitlement (this can be done with the in-app signer \[coming soon] or Feather and a development certificate, or for free utilizing a PC and [SideStore](https://sidestore.io/)), and enable Developer Mode on your iOS/iPadOS device (found at the bottom of Settings ➡️ Privacy & Security). Then, follow the instructions below to create and import your pairing file.

---

## Installation Instructions

### macOS

1. Download [idevice_pair for macOS](https://github.com/jkcoxson/idevice_pair/releases/latest/download/idevice_pair--macos-universal.dmg).
2. Open the Disk Image and drag `idevice pair` to `Applications`.

### Windows (64-bit)

1. Ensure [iTunes](https://apple.com/itunes/download/win64) is installed from from Apple's website.
2. Download [idevice_pair for Windows](https://github.com/jkcoxson/idevice_pair/releases/latest/download/idevice_pair--windows-x86_64.exe) and move it somewhere you will remember it.

### Linux

1. Ensure usbmuxd is installed and up to date on your machine by running `sudo apt install -y usbmuxd` in the Linux terminal.
2. Download the version of idevice_pair for Linux ([x86_64](https://github.com/jkcoxson/idevice_pair/releases/latest/download/idevice_pair--linux-x86_64.AppImage) or [AArch64](https://github.com/jkcoxson/idevice_pair/releases/latest/download/idevice_pair--linux-aarch64.AppImage)) that corresponds to your PC's architecture. Move it somewhere you will remember it, and make it executable.

---

## Pairing Instructions

1. Connect your secondary device to your computer via cable. If a prompt appears, select `trust` and type in your passcode.
2. Unlock your device, then open `idevice_pair` and select your device in the drop-down menu.
3. Ensure your device is unlocked and opened to the home screen, then select `load`. If a prompt appears on your device, tap `trust` and type in your passcode. Your pairing file should appear.
4. Ensure your device is still open to the home screen, then scroll down and select `install` below "StikDebug". `Success` should appear in green.
