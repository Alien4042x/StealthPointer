# StealthPointer

[![macOS](https://img.shields.io/badge/macOS-11.0+-blue?style=flat-square&logo=apple)](https://www.apple.com/macos/)
[![C++](https://img.shields.io/badge/C++-20-blue?style=flat-square&logo=cplusplus)](https://isocpp.org/)
[![Release](https://img.shields.io/github/v/release/Alien4042x/StealthPointer)](https://github.com/Alien4042x/StealthPointer/releases)
[![Downloads](https://img.shields.io/github/downloads/Alien4042x/StealthPointer/total)](https://github.com/Alien4042x/StealthPointer/releases)

**StealthPointer** is a lightweight native macOS menu bar app for hiding and showing the mouse cursor with global hotkeys, optional game profiles, and an auto-hide timer.

It is mainly built for Wine, CrossOver, WineForge, GPTK, and other game setups where the macOS cursor can stay visible, reappear after focus changes, or get in the way near the top of the screen.

## Features

- Global hide/show hotkeys, default `F1` / `F2`.
- Remappable hotkeys from the Settings window.
- StealthPointer Hub with Dashboard, Game Profiles, Display Setup, and Settings.
- Dashboard status for active profile, manual keys, and auto-hide state.
- Game Profiles with built-in Action and Strategy presets.
- Own Games profiles with saved custom key rules per game.
- Virtual keyboard editor for choosing show and hide cursor keys visually.
- Optional auto-hide timer with a configurable delay.
- Experimental display setup for saving, applying, and restoring macOS display modes.
- Native menu bar app with no background daemon.

## Game Profiles

Game Profiles add key-based cursor rules on top of the manual hotkeys. You can still use `F1` / `F2` when you want full manual control, or enable a profile when selected keys should show or hide the cursor automatically.

Example: inventory, map, journal, or menu keys can show the cursor, while movement/gameplay keys can hide it again.

Use Action or Strategy as built-in presets, or use Own Games to save custom rules for specific games.

## Auto-hide

Auto-hide is optional. When enabled, StealthPointer hides the cursor after the selected delay.

Press your configured show cursor hotkey to bring the cursor back temporarily. The default is `F2`, but it can be changed in Settings. The cursor stays visible for the time set by the auto-hide slider, then hides again.

This is useful if you want the cursor to disappear automatically but still need a short window to quit the app, change settings, or interact with macOS. Very short delays, such as 1 second, are not recommended because they give you almost no time to interact with macOS or quit the app.

## Setup Display (Experimental)

Setup Display can save your current macOS display mode, apply a selected resolution before launching a game, and restore the saved mode afterward.

This is experimental because fullscreen and borderless behavior depends heavily on the game, Wine/CrossOver, and macOS display handling. For best results, apply the macOS resolution first, then choose the same resolution inside the game.

## Usage

1. Launch StealthPointer from macOS.
2. Use `F1` to hide the cursor and `F2` to show it again.
3. Open the Hub from the menu bar icon.
4. Use Settings to change manual hotkeys and auto-hide.
5. Use Game Profiles if you want key-based cursor behavior per game.

## Download

[Releases](https://github.com/Alien4042x/StealthPointer/releases)

## Why?

macOS often keeps the cursor visible in fullscreen, borderless, or Wine-based games. StealthPointer gives you direct control without kernel extensions, background daemons, or changes to Wine itself.

## Troubleshooting

### Cursor reappears after changing resolution

Set the same resolution in macOS System Settings and inside the game before launching or entering fullscreen. macOS can reset display modes when resolutions differ, which may force the system cursor to reappear.

StealthPointer can hide and show the cursor, but it cannot fully control display-mode switches performed by macOS, Wine, CrossOver, WineForge, GPTK, or the game itself.

### Fullscreen causes flicker, cursor resets, or minimization

For better stability, try Borderless Windowed or Full Borderless Screen mode instead of traditional fullscreen. Many Wine-based games handle borderless modes more predictably on macOS.

## License

See [LICENSE.txt](LICENSE.txt) for full terms. Non-commercial use only.

---

Created by [Radim Veselý](https://github.com/Alien4042x/), 2025.
