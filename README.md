# Battle Network GBA for Android

**v0.2.2 preview** · Android 7.0 or later · ARM64

Unofficial standalone Android apps for the ten GBA editions of Mega Man Battle Network 1–6, plus Mega Man Battle Chip Challenge. Each APK has its own launcher and private save storage. The apps use the mGBA emulator with an SDL2 Android frontend. Commercial ROMs and the Nintendo GBA BIOS are absent from the download.

## Pick your edition

| Install the APK matching your cartridge | USA | Europe | Japan |
| --- | --- | --- | --- |
| Battle Network 1 | AREE | AREP | AREJ |
| Battle Network 2 | AE2E | AM2P | AE2J |
| Battle Network 3 Blue | A3XE | A3XP | A3XJ |
| Battle Network 3 White | A6BE | A6BP | A6BJ |
| Battle Network 4 Red Sun | B4WE | B4WP | B4WJ |
| Battle Network 4 Blue Moon | B4BE | B4BP | B4BJ |
| Battle Network 5 Team Protoman | BRBE | BRBP | BRBJ |
| Battle Network 5 Team Colonel | BRKE | BRKP | BRKJ |
| Battle Network 6 Cybeast Gregar | BR5E | BR5P | BR5J |
| Battle Network 6 Cybeast Falzar | BR6E | BR6P | BR6J |
| Battle Chip Challenge | A89E | A89P | A89J |

Cartridge IDs are based on the [Game Boy hardware database](https://gbhwdb.gekkio.fi/cartridges/gba.html) and the [Rockman EXE Zone cartridge survey](https://forums.therockmanexezone.com/mmbn-serial-number-survey-t4325.html).

## Install and play

1. Download the APK for your edition from [v0.2.2 Releases](https://github.com/GhostScitSMT/Mega-Man-BN-Series-Android-Ports-/releases/tag/V0.2.2). If you already have a preview installed, choose **Update** to keep your imported game and saves. If Android asks, allow installs from the app you opened the APK with.
2. Open the game’s launcher and choose **Choose game file**. Select your own matching `.gba` cartridge dump or a ZIP containing it. The launcher checks the header and copies the file to private storage.
3. Select **Play**. Use the controller or touch controls. The **TOUCH** button toggles the on-screen buttons, and **MENU** pauses the game and lets you return to the launcher.

The handheld layout puts GBA **A** on the right face button and **B** on the bottom. Use the game’s ordinary save function. **Save files** in the launcher imports and exports `.sav` battery saves. Each installed edition maintains separate saves, with separate save files for each cartridge region. Existing collection or recomp saves are not imported automatically.

## Optional GBA BIOS

Games can run with just a matching ROM. mGBA uses built-in routines to handle GBA startup and system calls when you play without an imported BIOS. An original GBA BIOS dump is recommended if you want startup and system behavior closer to the real hardware.

To add one, open **GBA BIOS → Import BIOS** and select your own standard 16 KB dump. The app verifies the file and enables it for that edition. Use the same menu to disable it or enable the original startup animation. The animation is off by default. Each standalone app stores its BIOS and settings separately.

## Credits

Android packaging and edition launchers by GhostScitSMT. The runtime uses [mGBA](https://github.com/mgba-emu/mgba) by Jeffrey Pfau and contributors under MPL 2.0, the [Gitsnup SDL2 Android frontend](https://github.com/Gitsnup/mgba-android/tree/8099fa2e0ec394ab57f99babec851480079f7f99), and [SDL2](https://github.com/libsdl-org/SDL/releases/tag/release-2.32.10) under the zlib license. See `NOTICE.txt` and the license files. Mega Man and the original games belong to Capcom.
