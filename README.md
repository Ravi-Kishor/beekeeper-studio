# 🐝 beekeeper-studio-bin (Prebuilt Arch Package)

Prebuilt Arch Linux package for **Beekeeper Studio**, built automatically from official upstream releases and published via GitHub Releases.

No AUR.  
No manual builds.  
No Electron compilation.

Repository:  
https://github.com/Ravi-Kishor/beekeeper-studio/

---

## 📦 Package

| Package | Description |
|----------|------------|
| beekeeper-studio-bin | Modern SQL editor and database manager (official binary) |

Build includes:

- Latest upstream stable release
- Official upstream AppImage
- Automatically packaged via GitHub Actions
- Pacman-managed install

---

# 🚀 Install / Update

Download and install the latest release:

```bash
LATEST=$(curl -s https://api.github.com/repos/Ravi-Kishor/beekeeper-studio/releases/latest | jq -r '.assets[].browser_download_url')

curl -LO "$LATEST"
sudo pacman -U beekeeper-studio-bin-*.pkg.tar.zst
```

Or download manually from:

https://github.com/Ravi-Kishor/beekeeper-studio/releases

---

## 🧠 What This Package Is

This is a **pacman-managed wrapper package** around the official AppImage.

Installed structure:

```
/usr/lib/beekeeper-studio/beekeeper.AppImage
/usr/bin/beekeeper-studio
```

Pacman handles:

- Installation
- Upgrades
- Removal
- Version tracking

The application itself is the official upstream binary.

---

## 🏗 Build Info

- Built inside Arch Linux container
- Official upstream AppImage used
- No source compilation
- Debug package disabled
- Clean minimal packaging

---

## 🔄 Automation

This repository:

- Checks upstream every 12 hours
- Builds automatically if new version exists
- Publishes GitHub Release
- Skips rebuild if version already released

---

## ⚠ Requirements

Arch Linux only.

Requires:

- pacman
- curl
- jq
- sudo

Runtime dependencies:

- gtk3
- nss
- libxss

---

## 📚 About Beekeeper Studio

Beekeeper Studio is a modern SQL editor and database manager.

Supports:

- MySQL
- MariaDB
- PostgreSQL
- SQLite
- SQL Server

Upstream project:

https://github.com/beekeeper-studio/beekeeper-studio
