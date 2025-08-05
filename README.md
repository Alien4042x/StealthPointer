# 👁️‍🗨️ StealthPointer

[![Release](https://img.shields.io/github/v/release/Alien4042x/StealthPointer)](https://github.com/Alien4042x/StealthPointer/releases)
[![Downloads](https://img.shields.io/github/downloads/Alien4042x/StealthPointer/total)](https://github.com/Alien4042x/StealthPointer/releases)

**StealthPointer** is a lightweight macOS menubar utility that allows you to hide and show your mouse cursor using global hotkeys.

## ✨ Features

- Global hotkeys for hiding/showing the cursor (default: F1 / F2)
- Customizable hotkeys (Cmd/Ctrl/Alt + any key)
- Simple and clean macOS menubar integration
- Optimized for Wine gaming
- No background processes or daemons – runs only in the menubar

## ⚙️ Usage

1. Launch the app – icon appears in the top macOS menu bar.
2. Press `F1` to hide the cursor, `F2` to show it again.
3. Click **Settings** in the menu to change hotkeys.

## 📥 Download

> 👉 [Releases](https://github.com/Alien4042x/StealthPointer/releases)

## 🧠 Why?

macOS often keeps the cursor visible in fullscreen or remote apps (like Wine).
This tool gives you control – without hacks or kernel extensions.

## 🔒 License

See [LICENSE.txt](LICENSE.txt) for full terms – non-commercial use only.

## ⚠️ From version 1.0.1

To improve compatibility with fullscreen Wine / CrossOver games and ensure reliable cursor recovery (F2),
the default behavior has changed:
- The system cursor is now always visible after launching the app.
- You’ll need to manually hide it using F1 when entering gameplay.
- This gives you full control but may feel inconvenient in games with frequent UI switches (e.g. survival/crafting games).

💡 We know this isn’t ideal — but right now it’s the most stable workaround.
Automatic detection (like combat/menu state) isn’t possible due to system limitations.

---

Created by [Radim Veselý](https://github.com/Alien4042x/), 2025.
