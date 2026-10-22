# BoltSweep releases

Installers for **[BoltSweep](https://boltsweep.com)**, a fast, private desktop email client for Windows, macOS and Linux. It has Outlook’s layout and keyboard shortcuts and works with Microsoft 365, Outlook.com, Gmail and any IMAP account. It is free for one account.

**Download:** https://boltsweep.com/download · **What’s new:** https://boltsweep.com/changelog

## Install

### Linux

One command, without root. It puts the AppImage in `~/Applications`, checks its checksum and adds BoltSweep to your app menu:

```bash
curl -fsSL https://boltsweep.com/install.sh | bash
```

AppImages need FUSE 2 to start:

| Distribution | Command |
|---|---|
| Arch, Manjaro, CachyOS, EndeavourOS | `sudo pacman -S --needed fuse2` |
| Ubuntu 24.04+, Debian 13 | `sudo apt install libfuse2t64` |
| Ubuntu 22.04, Debian 12 | `sudo apt install libfuse2` |
| Fedora | `sudo dnf install fuse-libs` |

You can also use packages from the [latest release](https://github.com/evaildev/boltsweep-releases/releases/latest):

```bash
sudo apt install ./BoltSweep_*_amd64.deb      # Ubuntu, Debian, Mint
sudo dnf install ./BoltSweep-*.x86_64.rpm     # Fedora, openSUSE
```

### Windows

Run `BoltSweep_<version>_x64-setup.exe` from https://boltsweep.com/download. The installer isn’t code-signed yet, so if SmartScreen says *Windows protected your PC*, click **More info → Run anyway**.

### macOS

Open `BoltSweep_<version>_universal.dmg` (Apple Silicon and Intel, macOS 11+) and drag BoltSweep to Applications. The first time you open it, go to **System Settings → Privacy & Security** and click **Open Anyway**.

## Updates

BoltSweep updates itself. Every release also has `SHA256SUMS` (from 0.5.0), and the `.sig` files are the updater’s signatures.

## About this repository

This repository only holds the release files and update information. BoltSweep is closed source. For questions and support, email hello@boltsweep.com.
