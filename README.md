# Animal-Crossing-VR-Launcher
Animal Crossing VR Launcher is for the meta quest 3 First-person VR, tracked tools, and repaired scenery. Bring your own legally dumped rom.

-  supported image file: `.iso`, `.gcm`, or `.ciso`.
- For installing a sideloaded APK, a USB-connected computer with Android platform tools/ADB or a compatible sideloading app.

**No game ROM, Nintendo game assets, or personal save files are included.** The user must provide their own game image.

## Install on Quest

1. Download the latest successful **Animal Crossing Quest APK** if one is available.
2. Enable Developer Mode on your Quest and authorize USB debugging.
3. Install the APK using SideQuest, Meta Quest Developer Hub, or ADB.
4. Put your own supported disc image somewhere accessible to the headset's file picker.
5. Launch **Animal Crossing**, choose the game-file import option, and select your disc image.
6. Wait for import and validation to finish, then start the game.

The APK is standalone after installation; the computer is only needed for sideloading if you are not using another supported installation method.

### Updating

Install a newer APK over the existing app using the same signing key. Do not uninstall the app or clear its storage if you want to preserve the imported game and saves. Export a backup before major updates whenever possible.

## Build from source

The workflow checks out the source, prepares the Android toolchain, fetches pinned SDL and OpenXR dependencies, runs package/data/RVZ tests, builds the APK, and uploads the APK with a build receipt and SHA-256 checksum.

## Documentation

- [Quest installation guide](quest/INSTALL.md)
- [Manual install, ROM transfer, and save backups](quest/MANUAL.md)
- [Quest build instructions](quest/BUILDING.md)
- [Quest architecture](quest/ARCHITECTURE.md)
- [Quest rewrite plan and milestones](docs/QUEST3_REWRITE.md)
- [Frequently asked questions](FAQ.md)

## Current development areas

Development is ongoing across:

- Player body, arms, and controller-driven movement.
- VR inventory and collection-page interaction.
- Sky and cloud rendering.
- Environment and scenery fixes.
- Launcher usability, save management, and diagnostics.
- Stability, crash reporting, and Quest lifecycle handling.

## Reporting a problem

When reporting a crash or other issue, include:

1. Quest model and OS version, if known.
2. The APK build or GitHub Actions run you installed.
3. What you were doing immediately before the issue.
4. Whether it happens every time or only sometimes.
5. The diagnostics export from the launcher, if the app can still be opened.

Please do not upload or share your game image or personal save files in an issue. Diagnostics may contain device/app information and runtime logs; review them before sharing publicly.

## Credits and legal

This project builds on the Animal Crossing decompilation and the existing PC port work. See the repository history, source headers, and [LICENSE](LICENSE) for attribution and licensing details.

Animal Crossing and related trademarks and game content are owned by Nintendo. This is an unofficial fan project and is not affiliated with, endorsed by, or sponsored by Nintendo. The project does not distribute Nintendo game files; users must supply their own legally obtained game image.
