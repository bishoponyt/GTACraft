# GTACraft

**Grand Theft Auto V Legacy × Minecraft Java passthrough**

GTACraft runs a separate Minecraft Java profile alongside GTA V Legacy and composites Minecraft into GTA's view. GTA supplies the world and camera; Minecraft supplies its blocks, items, and mobs.

The v0.1.2 passthrough is working. Known issues are listed under [Compatibility and safety](#compatibility-and-safety).

DISCLAIMER: This mod uses AI-assisted tools to develop and maintain. This is not affiliated with Rockstar Games, Mojang, Microsoft, or any other companies related to the games.

## Screenshots

Screenshots are coming soon. This section will be updated when captures are available.

<!-- Add captures under screenshots/ and replace the note above. Example:
![GTACraft in Los Santos](screenshots/gtacraft-los-santos.png)
-->

## Prerequisites

- Windows 10 or 11.
- GTA V **Legacy** installed on the computer.
- A Microsoft account with Minecraft Java Edition entitlement.
- Internet access during setup so the installer and Prism Launcher can retrieve required components and Minecraft files.

## Requirements

- GTA V Legacy game build **1.0.3889.0**. The selected GTA folder must contain `GTA5.exe`.
- ScriptHookV **3889.0.1158.13** and its ASI loader.
- ReShade **6.8.0** with add-on support.
- Minecraft Java Edition **26.3**, Fabric Loader **0.19.5**, and Fabric API **0.161.0+26.3**.
- Prism Launcher **11.1.1** for the separate Minecraft profile.

The setup program downloads the required launcher and mod dependencies when installing; GTA V and Minecraft game files are not included in the release archive.

## Install Instructions

1. Open the repository's **Releases** page and download `GTACraft-v0.1.2-public-release.zip`.
2. Extract the ZIP completely.
3. Drag the GTA V Legacy folder containing `GTA5.exe` onto `GTACraft-Setup.exe`, or run the setup program and browse to that folder.
4. Choose **Install GTACraft** and let setup finish.
5. When Prism Launcher opens, approve the GTACraft profile import, sign in with the Microsoft account that owns Minecraft Java Edition, and launch the GTACraft profile.
6. After Minecraft has loaded, start GTA V manually and choose **Story Mode**. Keep GTA windowed and turn off **Pause game on focus loss**.

## Uninstall Instructions

1. Close GTA V, Minecraft, and Prism Launcher.
2. Run `GTACraft-Setup.exe` again and select the same GTA V Legacy folder.
3. Choose **Uninstall from GTA**.

Uninstall removes GTACraft files only when their contents still match the installation record; changed files are left in place. The separate Minecraft profile, worlds, and sign-in data are kept by default. To remove that data too, turn off the keep-data option and confirm the additional prompt.

## Compatibility and safety

- **GTA V Legacy only.** GTA V Enhanced is not supported by this release.
- **Story Mode only. Never enter GTA Online with mod files installed.** BattlEye is disabled while GTACraft is installed.
- **Known issues in v0.1.2:**
  - The Minecraft pause menu and Minecraft-related controls require Alt+Tab into Minecraft, except for the hotbar and action buttons.
  - The player skin does not display in GTA V.
  - These issues are planned for future updates.
- Windows may show a SmartScreen warning because the setup executable is not code-signed.
- The release archive does not contain GTA V or Minecraft game assets. Keep the included `LICENSE` and `THIRD_PARTY_NOTICES.md` with redistributed copies.
- GTACraft is an unofficial fan project and is not affiliated with Rockstar Games, Take-Two Interactive, Mojang Studios, or Microsoft.

For installation details and credits, see the `README.md`, `LICENSE`, and `THIRD_PARTY_NOTICES.md` included in the release archive.
