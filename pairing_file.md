## Pairing Guide

idevice_pair allows us to create a pairing file for programs like StikDebug to talk to your device remotely. This pairing file is device-specific, time-specific and required to use StikDebug, otherwise StikDebug will not function correctly. Caution: this pairing file can and will expire randomly, requiring you to recreate it. This is due to Apple's systems and there is nothing we can do about it.

---
### Prerequisites
First, set a passcode on your device, sideload an app with the `get-task-allow` entitlement (this can be done with the in-app signer \[coming soon, in the meantime use Feather] and a development certificate, or for free utilizing a PC and [SideStore](https://sidestore.io/)), and enable Developer Mode on your iOS/iPadOS device (found at the bottom of Settings → Privacy & Security). Then, follow the instructions below to create and import your pairing file.

### Installation Instructions
#### macOS
1. Download [idevice_pair for macOS](https://github.com/jkcoxson/idevice_pair/releases/latest/download/idevice_pair--macos-universal.dmg)
2. Open the Disk Image and drag `idevice_pair` to `Applications`

#### Windows
1. Install [iTunes](https://apple.com/itunes/download/win64) from Apple's website
2. Download [idevice_pair for Windows](https://github.com/jkcoxson/idevice_pair/releases/latest/download/idevice_pair--windows-x86_64.exe) and save it to a memorable location

#### Linux
1. Install usbmuxd: 
   ```bash
   sudo apt install -y usbmuxd
   ```
2. Download idevice_pair for your architecture and save it to a memorable location:
   - [x86_64](https://github.com/jkcoxson/idevice_pair/releases/latest/download/idevice_pair--linux-x86_64.AppImage)
   - [AArch64](https://github.com/jkcoxson/idevice_pair/releases/latest/download/idevice_pair--linux-aarch64.AppImage)
3. Make the downloaded file executable

### Pairing Instructions

1. **Connect your device** to your computer via USB cable
   - If prompted, tap `Trust` and enter your passcode
2. **Open idevice_pair** and select your device from the dropdown menu
3. **Load pairing file**: 
   - Ensure your device is unlocked and on the home screen
   - Click `Load`
   - If prompted, tap `Trust` and enter your passcode
4. **Install to StikDebug**:
   - Keep your device unlocked and on the home screen
   - Scroll down and click `Install` under "StikDebug"
   - You should see `Success` appear in green
