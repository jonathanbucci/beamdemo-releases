<img src="assets/beamdemo-icon.png" alt="BeamDemo" width="88" align="right">

# BeamDemo Releases

Public installer downloads for **BeamDemo** — a standalone app for running live
lighting demos and presentations.

## Download

**[Get the latest release](../../releases/latest)** — installers for Windows,
macOS, and Linux.

BeamDemo requires a **license code** to activate. Don't have one yet? Contact the
BeamDemo team.

## Choose your installer

| Platform | File | Notes |
|---|---|---|
| **Windows** | `BeamDemo_<version>_x64-setup.exe` | Recommended. A `.msi` is also provided. |
| **macOS** | `BeamDemo_<version>_universal.dmg` | Universal — Intel + Apple Silicon. |
| **Linux** | `BeamDemo_<version>_amd64.AppImage` | A `.deb` is also provided. |

## Installation notes (alpha builds)

Alpha builds are **not yet code-signed**, so your OS may warn you the first time.

- **macOS:** open the `.dmg` and drag BeamDemo to Applications. If the first launch
  is blocked, open **System Settings → Privacy & Security**, scroll to the message
  about BeamDemo, and click **Open Anyway** — then confirm. You only need to do this
  once. (The older *right-click → Open* trick no longer bypasses Gatekeeper on
  macOS 15 Sequoia and later.) If macOS instead reports the app is
  *"damaged and can't be opened,"* the download's quarantine flag needs clearing —
  open **Terminal** and run this once, then reopen the app:

  ```
  xattr -dr com.apple.quarantine /Applications/BeamDemo.app
  ```

- **Windows:** if SmartScreen shows *"Windows protected your PC,"* click
  **More info → Run anyway.** Installing on a machine that has **no internet
  connection *and* lacks the Microsoft WebView2 runtime** (uncommon — WebView2 ships
  with Windows 11 and most updated Windows 10) needs an internet connection once, so
  the installer can download WebView2.

- **Linux:** the `.deb` is recommended where available (Debian/Ubuntu) — it pulls in
  the media codecs and installs the Stream Deck access rule for you. The `.AppImage`
  is self-contained and runs anywhere; after connecting a Stream Deck on Linux you may
  need a udev rule for it to open (the `.deb` installs this automatically).

---

This repository hosts **release binaries only** — BeamDemo's source code is private.
© BeamDesk contributors.
