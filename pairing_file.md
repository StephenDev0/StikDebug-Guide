## Pairing Instructions

### Downloads
- **Windows**: [jitterbugpair-win64.zip](https://github.com/osy/Jitterbug/releases/download/v1.3.1/jitterbugpair-win64.zip)
- **macOS**: [jitterbugpair](https://github.com/SideStore/SideStore-Docs/releases/download/need-a-place-to-put-jittterbug/jitterbugpair)
- **Linux**: [jitterbugpair-linux.zip](https://github.com/osy/Jitterbug/releases/download/v1.3.1/jitterbugpair-linux.zip)

---

### For Windows

1. **Extract** `jitterbugpair-win64.zip`.
2. **Set a passcode** for your device if you haven't already. Unlock your device and connect it to your computer via cable. When a prompt appears, tap "Trust."
3. Open your device to the homescreen.
4. In File Explorer, locate `jitterbugpair.exe` and run it by double-clicking or right-clicking and selecting "Open".
5. JitterbugPair will generate a **pairing file** in the same folder. This file will have the extension `.mobiledevicepairing`.
6. **Transfer the pairing file** to your iOS device using One/iCloud/Google Drive, email, or any other method. For best results, compress the file into a .zip folder first.

---

### For macOS

1. **Extract** `Jitterbugpair-macos.zip` (if applicable).
2. **Set a passcode** for your device if you haven't already. Unlock your device and connect it to your computer via cable. When a prompt appears, tap "Trust."
3. Open your device to the homescreen.
4. Find the extracted `jitterbugpair` file (it should have a black and green icon).
5. Open Terminal (in Launchpad, it's in the "Utilities" folder).
6. Drag the `jitterbugpair` file into Terminal and press "Return" or Enter.
7. If you get "macOS cannot verify that this app is free from malware":
   - Go to System Settings > Privacy & Security
   - Scroll down to the message about the app
   - Click "Open Anyway," if the program doesn't run automatically, try manually running it again
8. JitterbugPair will generate a **pairing file** with the extension `.mobiledevicepairing` to your user's home folder.
9. If you can't find the pairing file:
   - Copy the name of the pairing file generated
   - Paste it into Finder
   - If you ran the program more than once, all pairing files for your device should appear since they share the same name
10. **Transfer the pairing file** to your iOS device using AirDrop, iCloud/One/Google Drive, email, or any other method. For best results, compress the file into a .zip folder first.

---

### For Linux

1. **Extract** `jitterbugpair-linux.zip`.
2. Open a terminal in the extracted directory.
3. Make the program executable:
   ```bash
   chmod +x ./jitterbugpair
   ```
4. **Set a passcode** for your device if you haven't already. Unlock your device and connect it to your computer via cable. When a prompt appears, tap "Trust."
5. Open your device to the homescreen.
6. Execute the program:
   ```bash
   ./jitterbugpair
   ```
7. JitterbugPair will generate a **pairing file** with the extension `.mobiledevicepairing`.
8. **Transfer the pairing file** to your iOS device using your preferred method. For best results, compress the file into a .zip folder first.

> [!TIP]
> When using cloud storage, the file extension might change (usually to .txt). It is always recommended to zip your pairing file before transferring it. StikDebug only accepts `.mobiledevicepairing` or `.plist` files.

---

### On your iOS device

1. In the **Files app**, locate your newly-generated pairing file. (If zipped, long-press your zipped pairing file and select **Uncompress**.)
2. Launch the **StikDebug** app.
   - If the app doesn't appear, restart your device.
3. Upon launching the app, tap **Import Pairing File**, then navigate to and select your **unzipped pairing file**.
4. StikDebug is now ready for use.
