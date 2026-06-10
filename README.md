<div align="center">

# Balatro GBA - Browser Edition

**Play the Balatro GBA fan demake instantly in your browser. No download, no install, no setup.**

[![Play Now](https://img.shields.io/badge/PLAY%20NOW-outblade.github.io%2Fbalatro--web-e8a838?style=for-the-badge&labelColor=0d0d1a)](https://outblade.github.io/balatro-web/)

[![GitHub Pages](https://img.shields.io/github/deployments/OutBlade/balatro-web/github-pages?label=GitHub%20Pages&style=flat-square)](https://outblade.github.io/balatro-web/)
[![ROM Source](https://img.shields.io/badge/ROM-GBALATRO%2Fbalatro--gba-blue?style=flat-square)](https://github.com/GBALATRO/balatro-gba)
[![Emulator](https://img.shields.io/badge/Emulator-EmulatorJS-orange?style=flat-square)](https://github.com/EmulatorJS/EmulatorJS)
[![Stars](https://img.shields.io/github/stars/OutBlade/balatro-web?style=flat-square)](https://github.com/OutBlade/balatro-web/stargazers)

[![Preview](https://outblade.github.io/balatro-web/social.png)](https://outblade.github.io/balatro-web/)

*Click the image to play*

</div>

---

## Why this exists

Balatro is the poker roguelike everyone is hooked on. The community built an impressive Game Boy Advance demake - but playing it normally means downloading a ROM and setting up an emulator. This project removes all of that friction: one link, and you are drawing cards three seconds later. On your PC, your phone, or that locked-down work laptop.

**[outblade.github.io/balatro-web](https://outblade.github.io/balatro-web/)**

- **Zero setup** - runs entirely in the browser via WebAssembly
- **Works everywhere** - PC, Mac, Android, iOS
- **Your progress is saved** - localStorage keeps your run between sessions
- **Fullscreen, no black bars** - the game scales to fill any screen
- **Touch controls on mobile** - built into EmulatorJS

---

## Controls

| Key | GBA Button | Action |
|-----|-----------|--------|
| `Arrow keys` | D-Pad | Navigate menus / move cursor |
| `Space` | A | Select / confirm card |
| `Escape` | B | Deselect all cards |
| `Enter` | L | Play Hand / **Sell Joker** |
| `Backspace` | R | Discard |
| `Shift` | Select | GBA Select |
| `Tab` | Start | GBA Start / pause |
| `F` or `F11` | - | Toggle fullscreen |

The bindings are designed to feel close to the Steam version: `Enter` to play, `Backspace` to discard, arrow keys to navigate.

### Selling and moving jokers

Some actions depend on where your cursor is:

- **Sell a joker** - press `Up` to move the cursor onto the joker row (in the shop or during a round), highlight the joker, then press `Enter` (GBA L).
- **Move / swap jokers or cards** - highlight one, **hold** `Space` (GBA A), then use the arrow keys.

---

## Android APK

Prefer playing offline on Android? Download the APK directly from this repo - no Play Store needed.

[![Download APK](https://img.shields.io/badge/Download-Balatro.apk-e8a838?style=for-the-badge&labelColor=0d0d1a)](https://github.com/OutBlade/balatro-web/raw/main/Balatro.apk)

> Install tip: enable *"Install from unknown sources"* in your Android settings before installing.

---

## Tech stack

| Component | Details |
|-----------|---------|
| ROM | [balatro-gba v1.1](https://github.com/GBALATRO/balatro-gba) by GBALATRO and contributors |
| Emulator | [EmulatorJS](https://github.com/EmulatorJS/EmulatorJS) (mGBA core) |
| Hosting | GitHub Pages - the whole site is a single `index.html` |

---

## Found a bug? Have an idea?

[Open an issue](https://github.com/OutBlade/balatro-web/issues) - gameplay bugs in the demake itself belong upstream at [GBALATRO/balatro-gba](https://github.com/GBALATRO/balatro-gba/issues), while anything about the browser wrapper (controls, scaling, saving, mobile) belongs here.

If this saved you an emulator setup, a star helps other people find it.

---

## Legal

This is a **non-profit fan project**. It is not affiliated with, endorsed by, or sponsored by Playstack or LocalThunk.

The original **Balatro** is a paid game - please support the developer:

[![Buy Balatro on Steam](https://img.shields.io/badge/Buy%20on-Steam-1b2838?style=flat-square&logo=steam)](https://store.steampowered.com/app/2379780/Balatro/)

The GBA demake ROM is sourced from [GBALATRO/balatro-gba](https://github.com/GBALATRO/balatro-gba) (MIT-licensed fan project).
