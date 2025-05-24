## Pairing Instructions

### Downloads
- **Windows**: [iDevicePair--windows-x86_64.exe](https://github.com/jkcoxson/idevice_pair/releases/latest/download/iDevicePair--windows-x86_64.exe)
- **macOS**: [iDevicePair--macos-universal.dmg](https://github.com/jkcoxson/idevice_pair/releases/latest/download/iDevicePair--macos-universal.dmg)
- **Linux**: (x86_64: [iDevicePair--linux-x86_64.AppImage](https://github.com/jkcoxson/idevice_pair/releases/latest/download/iDevicePair--linux-x86_64.AppImage) or AArch64: [iDevicePair--linux-aarch64.AppImage](https://github.com/jkcoxson/idevice_pair/releases/latest/download/iDevicePair--linux-aarch64.AppImage))
---

iDevice Pair allows us to create a pairing file for programs like StikDebug to talk to your device remotely. This is required to use StikDebug, otherwise it will not function.

### Windows

1. Install iTunes from Apple's website ([64-bit](https://apple.com/itunes/download/win64) or [32-bit](https://apple.com/itunes/download/win32)).
2. Download `iDevicePair--windows-x86_64.exe` (move it somewhere you won't lose it).
3. Connect your secondary device to your computer via cable. If a prompt appears, tap "trust" and type in your passcode.
4. Unlock your device, open iDevice Pair, and select your device in the drop-down menu.
5. Ensure your device is unlocked and opened to the home screen, then select "generate" (If also use an app such as SideStore which utilizes this pairing file, select "load" instead). When a prompt appears on your device, tap "trust". Your pairing file should appear.
6. Ensure your device is still open to the home screen, then scroll down to the StikDebug section and select "install". The word "success" should appear in green.

### macOS

1. Download `iDevicePair--macos-universal.dmg`. Open the file and drag `iDevice Pair` to your Applications folder.
3. Connect your secondary device to your computer via cable. If a prompt appears, tap "trust" and type in your passcode.
4. Unlock your device, open iDevice Pair, and select your device in the drop-down menu.
5. Ensure your device is unlocked and opened to the home screen, then select "generate" (If you also use an app such as SideStore which also utilizes this pairing file, select "load" instead). When a prompt appears on your device, tap "trust". Your pairing file should appear.
6. Ensure your device is still open to the home screen, then scroll down to the StikDebug section and select "install". The word "success" should appear in green.

### Linux

> [!TIP]
> The iDevice Pair instructions for Linux are a work-in-progress, though iDevice Pair is pretty intuitive if you want to give it a try without docs first. For now, instructions to create a pairing file using JitterbugPair for Linux are below!

These instructions expect that you are familiar with the linux commandline.

1. **Download** `jitterbugpair-linux.zip` from [here](https://github.com/osy/Jitterbug/releases/download/v1.3.1/jitterbugpair-linux.zip), then extract it.
2. Open a terminal in the extracted directory.
3. Make the program executable:
   ```bash
   chmod +x ./jitterbugpair
   ```
4. **Set a passcode** for your device if you haven't already. Unlock your device and connect it to your computer via cable. If a prompt appears, tap "trust" and type in your passcode.
5. Open your device to the homescreen.
6. Execute the program:
   ```bash
   ./jitterbugpair
   ```
7. The first time you execute the tool, you will get a prompt for your passcode on your secondary device. Type it in, then keep the screen on and unlocked and run the tool again. Type it in, then keep the screen on and unlocked and execute the tool again.
8. JitterbugPair will generate a **pairing file** with the extension `.mobiledevicepairing`.
9. Compress the file into a .zip folder. Then, **transfer the pairing file** to your iOS device using email, cloud storage, or another method you prefer. On your iOS/iPadOS device's Files app, long press on the file, then select "Uncompress". Inside StikDebug, select "Choose Pairing File", then select your unzipped pairing file.
