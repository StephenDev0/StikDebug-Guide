## Pairing Instructions

### Downloads
- **Windows**: [iDevicePair--windows-x86_64.exe](https://github.com/jkcoxson/idevice_pair/releases/latest/download/iDevicePair--windows-x86_64.exe)
- **macOS**: [iDevicePair--macos-universal.dmg](https://github.com/jkcoxson/idevice_pair/releases/latest/download/iDevicePair--macos-universal.dmg)
- **Linux**: (x86_64: [iDevicePair--linux-x86_64.AppImage](https://github.com/jkcoxson/idevice_pair/releases/latest/download/iDevicePair--linux-x86_64.AppImage) or AArch64: [iDevicePair--linux-aarch64.AppImage](https://github.com/jkcoxson/idevice_pair/releases/latest/download/iDevicePair--linux-aarch64.AppImage))

---

idevice pair allows us to create a pairing file for programs like StikDebug to talk to your device remotely. This is required to use StikDebug, otherwise it will not function.

---

First, set a passcode on your device, sideload an app with the get-task-allow entitlement, and enable Developer Mode on your iOS/iPadOS device (found in Settings -> Privacy & Security after sideloading an app). Then, follow the instructions below.

---

### Windows (64-bit)

1. Install [iTunes](https://apple.com/itunes/download/win64) from Apple's website.
2. Download `iDevicePair--windows-x86_64.exe` (move it somewhere you won't lose it).
3. Connect your secondary device to your computer via cable. If a prompt appears, tap `trust` and type in your passcode.
4. Unlock your device, then, in File Explorer, open `idevice pair` and select your device in the drop-down menu.
5. Ensure your device is unlocked and opened to the home screen, then select `load`. Your pairing file should appear.
6. Ensure your device is still open to the home screen, then scroll down to the StikDebug section and select `install`. The word "success" should appear in green.

---

### macOS

1. Download `iDevicePair--macos-universal.dmg`. Open the image and drag `idevice pair` to `Applications`.
2. Connect your secondary device to your computer via cable. If a prompt appears, tap `trust` and type in your passcode.
3. Unlock your device, then open `idevice pair` and select your device in the drop-down menu.
4. Ensure your device is unlocked and opened to the home screen, then select `load`. Your pairing file should appear.
5. Ensure your device is still open to the home screen, then scroll down to the StikDebug section and select `install`. The word "success" should appear in green.

---

### Linux

1. In the Linux terminal, run the following command to install usbmuxd:
```
sudo apt install -y usbmuxd
```
2. Download the version of `idevice pair` above that corresponds to your PC's architecture and make it executable.
3. Connect your secondary device to your computer via cable. If a prompt appears, tap `trust` and type in your passcode.
4. Unlock your device, then execute `idevice pair` and select your device in the drop-down menu.
5. Ensure your device is unlocked and opened to the home screen, then select `generate` (If already using an app such as SideStore which also utilizes a pairing file, select `load` instead). When a prompt appears on your device, tap `trust`. Your pairing file should appear.
6. Ensure your device is still open to the home screen, then scroll down to the StikDebug section and select `install`. The word "success" should appear in green.
