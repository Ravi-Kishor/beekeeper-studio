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
- Pacman-managed installation
- Debug package disabled

---

# 🚀 Install / Update (Recommended Method)

Install the updater:

```bash
curl -fLO https://raw.githubusercontent.com/Ravi-Kishor/beekeeper-studio/main/update-beekeeper
chmod +x update-beekeeper
sudo mv update-beekeeper /usr/local/bin/update-beekeeper
```

Then run:

```bash
update-beekeeper
```

---

## 🧠 What the updater does

- Detects installed version via pacman
- Fetches latest GitHub release
- Finds correct `.pkg.tar.zst` asset
- Lets you choose:
  - Update (skip if already latest)
  - Force install
- Downloads and installs automatically
- Cleans temporary files

---

## 📦 Manual Installation

You can also install manually from Releases:

https://github.com/Ravi-Kishor/beekeeper-studio/releases

Then:

```bash
sudo pacman -U beekeeper-studio-bin-*.pkg.tar.zst
```

---

## 🏗 Build Info

- Built inside Arch Linux container
- Official upstream AppImage used
- No source compilation
- No Electron toolchain required
- Clean minimal packaging
- Installed structure:

```
/usr/lib/beekeeper-studio/beekeeper.AppImage
/usr/bin/beekeeper-studio
```

---

## 🔄 Automation

This repository:

- Checks upstream every 12 hours
- Builds automatically when a new version is released
- Publishes a GitHub Release
- Skips rebuild if version already exists

---

## ⚠ Requirements

Arch Linux only.

Required tools for updater:

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
