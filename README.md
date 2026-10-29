# AoE:DE Mod Manager

A small Windows program to install, switch and remove mods for **Age of Empires: Definitive Edition**
(the 2018 remake of the first Age of Empires, Steam version).

**[Download the latest version from Releases](../../releases/latest)**: one file, `AoEDE_ModManager.exe`,
nothing to install.

## Online play

- **Visual mods** (graphics, sounds, interface) can be used in online play.
- **Data mods** (mods that change files in `Data\`, such as `empires.dat`) **will cause the game to crash in
  online play.** Use them in single-player only. Before playing online, untick them and press
  **Apply enabled mods** (or press **Restore originals**).

## What it does

- **Add** a mod from a `.zip` file. Only the files that belong in the game's folders are used; everything else
  in the zip is ignored.
- **Tick** the mods you want and press **Apply enabled mods**. Every game file is backed up before it is
  replaced.
- **Restore originals** puts every original game file back, checked against its backup.
- **Move up / down** decides which mod wins when two mods change the same file; **Conflicts...** lists them.
- **Remove** moves a mod's folder to the Recycle Bin (untick it and press Apply first).
- **Get Mods** opens the official Age of Empires mod website.
- **Launch Game** starts the game through Steam.
- While the game is running, the mod manager is locked so nothing changes under the game's feet.

## Install

1. Download `AoEDE_ModManager.exe` from **Releases**.
2. Put it in its own folder, for example `Documents\AoEDE Mod Manager`. Do not put it in the game folder.
3. Double-click it. It creates a `mods` folder next to itself.
   - If Windows shows "Windows protected your PC", click **More info > Run anyway**. The program is not
     code-signed yet, so Windows does not recognise it.
4. Check the **Game folder** at the top. The default is
   `C:\Program Files (x86)\Steam\steamapps\common\AoEDE`; use **Browse...** if yours is elsewhere.

Requirements: Windows 10 or 11 (64-bit) and the Steam version of Age of Empires: Definitive Edition.

## Uninstall

Press **Restore originals**, close the program, then delete its folder. If anything ever looks wrong, Steam can
repair the game: right-click the game > **Properties > Installed Files > Verify integrity of game files**.

## Problems

- *"Windows refused to write a game file"*: close the game, or right-click the program > **Run as administrator**.
- *Everything is greyed out*: the game is running. Close it and the program unlocks itself.

To report a problem, open an **Issue** here and include the first line of the program's log (for example
`AoE:DE Mod Manager 1.0 (build 7)`), what you clicked, and what happened. A screenshot helps.

## Legal

Free to download and use, see [LICENSE.txt](LICENSE.txt). This program contains no game files.
Age of Empires is a trademark of Microsoft. This project is not affiliated with or endorsed by Microsoft
or World's Edge.
