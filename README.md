# Tax Noir — desktop installers

This repository hosts **release builds only** of the Tax Noir desktop app, a film-noir tax-training
game. The source code is private.

**Download:** open [Releases](../../releases/latest) and pick the installer for your computer:

- **Mac:** `Tax-Noir-<version>-universal.dmg` (Apple silicon and Intel)
- **Windows:** `Tax-Noir-Setup-<version>.exe`

## First launch

The app is not yet signed with an Apple or Microsoft certificate, so your computer will warn you
once. The warning is about the missing certificate, not a broken download.

- **Mac:** drag Tax Noir to Applications and open it. macOS says it can't verify the app; click
  **Done** (or **Cancel**). Then open System Settings → Privacy & Security, scroll down to the
  message about Tax Noir and click **Open Anyway**, then confirm. On macOS 14 Sonoma and older you
  can instead right-click the app and choose **Open**. On macOS 15 Sequoia and later right-click →
  Open no longer gets past the warning; use **Open Anyway** in System Settings.

  If macOS still refuses (for example it says the app "is damaged"), open Terminal and run:

  ```bash
  xattr -dr com.apple.quarantine "/Applications/Tax Noir.app"
  ```

  This removes only the "downloaded from the internet" flag from this one app; it changes no other
  security settings. Then open Tax Noir as usual.
- **Windows:** when SmartScreen appears, click **More info → Run anyway**.

## Updates

- **Windows:** the app downloads new versions in the background and offers to restart.
- **Mac:** the app tells you when a new version exists and opens this page to download it.

> Tax Noir is a **proof of concept**. Its tax content has not been reviewed by a qualified tax
> professional and must not be used as advice.
