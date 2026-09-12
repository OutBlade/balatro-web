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
- **Save states** - use the emulator's Save State / Load State controls to continue a run
- **Fullscreen with the whole game visible** - preserves the GBA's 3:2 picture without cropping
- **Touch controls on mobile** - built into EmulatorJS

---

## Updated to GBALATRO v0.2.2

The browser edition now uses the [stable v0.2.2 ROM](https://github.com/GBALATRO/balatro-gba/releases/tag/v0.2.2), released August 11, 2026. Upstream changed its version numbering: **v0.2.2 is newer than the previous v1.1**.

Changes since the previously bundled ROM include shop joker descriptions, high-contrast and large-font cards, saved audio/readability settings, the completed main theme, improved seeded runs, an expanded game-over screen, and bug fixes.

The browser wrapper also fixes the A/L/R mappings, pins EmulatorJS to 4.2.3, and keeps the complete game image visible when the window is resized. The versioned ROM filename gives the new release its own cache and save-state name.

This is still a limited fan demake with 52 jokers. Native run loading and boss-blind effects are not complete in this release.

---

## Controls

| Key | GBA Button | Action |
|-----|-----------|--------|
| `Arrow keys` | D-Pad | Navigate menus / move cursor |
| `Space` | A | Select / confirm card |
| `Escape` | B | Deselect cards; hold over a shop joker to read its description |
| `Enter` | L | Play Hand / **Sell Joker** |
| `Backspace` | R | Discard |
| `Shift` | Select | GBA Select |
| `Tab` | Start | GBA Start |
| `F` or `F11` | - | Toggle fullscreen |

The bindings are designed to feel close to the Steam version: `Enter` to play, `Backspace` to discard, arrow keys to navigate.

### Selling and moving jokers

Some actions depend on where your cursor is:

- **Sell a joker** - press `Up` to move the cursor onto the joker row (in the shop or during a round), highlight the joker, then press `Enter` (GBA L).
- **Move / swap jokers or cards** - highlight one, **hold** `Space` (GBA A), then use the arrow keys.
- **Read a joker description** - highlight a joker in the shop and hold `Escape` (GBA B).

Use the emulator toolbar's **Pause** button to pause. Keyboard and controller bindings can be changed in **Control Settings**. If previously saved bindings override the defaults, select **Reset** there. Touch controls are provided by EmulatorJS.

### Saving and continuing a run

Native game saving currently preserves options; it does **not** provide a working run-resume feature. Closing or refreshing the page does not automatically preserve the current run.

1. Before leaving, use **Save State** in the emulator toolbar. By default this downloads a state file.
2. To continue, open the same ROM version and use **Load State** with that file.
3. For local browser slots, choose **Settings → Save States → Save State Location → Keep in Browser**, then use Save State / Load State. Keep a downloaded backup; clearing browser data can remove browser saves.

**Export Save File** exports the game's SRAM data, which is different from a full emulator state and is not a replacement for saving your run.

States from v1.1 are not guaranteed to work in v0.2.2. Use the [previous v1.1 browser version](https://outblade.github.io/balatro-web/?version=1.1) for old states. The old ROM filename and browser save namespace are retained; this update does not migrate or delete previous saves.

---

## Android APK

The existing Android APK is a separate legacy download. It has **not** been rebuilt for this browser update; use the browser link above for v0.2.2.

[![Download APK](https://img.shields.io/badge/Download-Balatro.apk-e8a838?style=for-the-badge&labelColor=0d0d1a)](https://github.com/OutBlade/balatro-web/raw/main/Balatro.apk)

> Install tip: enable *"Install from unknown sources"* in your Android settings before installing.

---

## Tech stack

| Component | Details |
|-----------|---------|
| ROM | [balatro-gba v0.2.2](https://github.com/GBALATRO/balatro-gba/releases/tag/v0.2.2) by GBALATRO and contributors |
| Emulator | [EmulatorJS 4.2.3](https://github.com/EmulatorJS/EmulatorJS/tree/v4.2.3) (mGBA core) |
| Hosting | GitHub Pages - the whole site is a single `index.html` |

The bundled `balatro-gba-0.2.2.gba` is the unmodified upstream release asset (5,061,324 bytes). SHA-256:

```text
c2ef394b332a973398f970c53398af2600bbcbf666cbe6f9aa0238457d3f9c94
```

---

## Found a bug? Have an idea?

[Open an issue](https://github.com/OutBlade/balatro-web/issues) - gameplay bugs in the demake itself belong upstream at [GBALATRO/balatro-gba](https://github.com/GBALATRO/balatro-gba/issues), while anything about the browser wrapper (controls, scaling, saving, mobile) belongs here.

If this saved you an emulator setup, a star helps other people find it.

---

## Legal

This is a **non-profit fan project**. It is not affiliated with, endorsed by, or sponsored by Playstack or LocalThunk.

The original **Balatro** is a paid game - please support the developer:

[![Buy Balatro on Steam](https://img.shields.io/badge/Buy%20on-Steam-1b2838?style=flat-square&logo=steam)](https://store.steampowered.com/app/2379780/Balatro/)

The GBA demake ROM is sourced from [GBALATRO/balatro-gba](https://github.com/GBALATRO/balatro-gba). See the upstream project's disclaimer and contribution scope. Rights to the original game remain with their respective holders.
