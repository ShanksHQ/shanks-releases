# Shanks releases

Downloads and in-app updates for Shanks, a local-first AI workspace for pentesters. This repository only holds release builds.

## Install

1. Download `Shanks_<version>_aarch64.dmg` from the [latest release](https://github.com/Majkie/shanks-releases/releases/latest). Shanks runs on Apple Silicon Macs with macOS 13 or newer.
2. Open the DMG and drag **Shanks** to **Applications**, replacing an older copy if you have one.
3. Shanks is not notarized by Apple, so macOS blocks the first launch. Open Shanks once, then go to **System Settings → Privacy & Security** and click **Open Anyway** next to the Shanks message. Alternatively, clear the download flag in Terminal:

   ```sh
   xattr -dr com.apple.quarantine /Applications/Shanks.app
   ```

Your projects, evidence and settings live in `~/Library/Application Support/dev.shanks.app` and stay in place when you install a newer version over an older one.

## Updates

Shanks 0.2.0 and newer check this repository for updates on start and every six hours (Settings → About → Updates, or **Check for updates** in the command palette). An update is installed only after you choose **Install and restart**, and only when it is signed with the Shanks release key.

After an update macOS may ask once whether Shanks can use its saved keys in the keychain. Choose **Always Allow**.

Coming from a build without updates (before 0.2.0)? Install the latest DMG over it once as described above; your data stays where it is.
