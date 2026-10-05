# GrandCraft
A working one-click installer for the Grand Theft Auto V x Minecraft passthrough mod.

GTACraft runs Minecraft Java alongside GTA V Legacy and composites Minecraft into GTA's view. GTA provides the city, terrain, camera, and host-game behavior; Minecraft provides its own blocks, items, and mobs.

## Install

1. Extract this archive.
2. Drag the GTA V Legacy folder containing `GTA5.exe` onto `GTACraft-Setup.exe`, or open the installer and choose that folder.
3. Select **Install GTACraft**. Setup supports GTA V Legacy build `1.0.3889.0`; it stops if the game build differs or a target file is already present.
4. Prism Launcher opens the isolated GTACraft Minecraft profile. Sign in with a Microsoft account that owns Minecraft Java Edition, approve the profile import if prompted, then launch the GTACraft instance.
5. After Minecraft finishes loading, start GTA V manually and select Story Mode. Keep GTA windowed and turn off “Pause game on focus loss.” The menu choice is intentionally manual.

The installer fetches ScriptHookV, the ReShade add-on runtime, Prism Launcher, and Fabric API from their respective distribution sites. Minecraft game files and its Java runtime are retrieved through Prism after account sign-in. This archive contains no GTA V or Minecraft game data and no ScriptHookV or ReShade runtime binaries.

## Uninstall

Run `GTACraft-Setup.exe`, select the same GTA folder, and choose **Uninstall from GTA**. It removes only files whose hashes still match the installation record; changed files are preserved. Minecraft worlds and sign-in data are kept by default. Deleting them requires unchecking the keep-data option and confirming a second prompt.

## Compatibility and safety

- GTA V Legacy `1.0.3889.0`; Story Mode only.
- ScriptHookV `3889.0.1158.13`; ReShade add-on `6.8.0`.
- Minecraft Java `26.3`; Fabric Loader `0.19.5`; Fabric API `0.161.0+26.3`.
- Do not enter GTA Online with modded files installed. BattlEye is disabled by the installed ScriptHookV arguments.
- This build compiled successfully but has not yet been validated in a live GTA Story Mode session. Treat it as an early community release.
- Windows may show a SmartScreen warning because the executable is not code-signed.

This is a binary installer release. The passthrough implementation is based on [rehan-remade/universal-modder](https://github.com/rehan-remade/universal-modder/tree/main/examples/minecraft-gta5-passthrough). See `LICENSE` and `THIRD_PARTY_NOTICES.md` for attribution.
