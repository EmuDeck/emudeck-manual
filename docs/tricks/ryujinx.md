# <img src="/assets/emulators/ryujinx.png" alt="EmuDeck guide" width="80" style="vertical-align: middle"> Ryujinx Tips and Tricks

[TOC]

---

### How to Configure Gyro



Gyro for Ryujinx requires SteamDeckGyroDSU. SteamDeckGyroDSU can be installed via EmuDeck, or it can be installed manually.

Visit [SteamDeckGyroDSU](../../emudeck-application/steamos/emudeck-application-101.md#steamdeckgyrodsu) to learn how to install and utilize SteamDeckGyroDSU.

---

### How to Configure Gyro With External Controllers



1. Switch to Desktop Mode
2. Exit out of Steam
   - You may exit out of Steam a couple of different ways:
     - Right click the `Steam` icon in your taskbar and click `Exit Steam`
     - Open Steam, click the `Steam` button in the top left, click `Exit`
     - Open a terminal (Konsole) and enter `killall -9 steam`
     - Do note that clicking the the `X` button in the top right of the Steam window **will not** exit out of Steam
   - Your controls will switch to `Lizard Mode`. Use `L2` to right click, `R2` to left click, and the `Right Trackpad` to move the mouse
   - You may also connect an external keyboard and mouse
3. Click the bluetooth icon in the bottom right of your taskbar and connect your controller
   <img src="https://github.com/dragoonDorise/EmuDeck/assets/108900299/24945d4c-df06-4fbe-9668-7becea0c5edb" height="300">
4. Open Ryujinx
5. Click `Options` at the top, click `Settings`
6. Click the `Input` tab on the top
7. Click `Configure` under `Player 1`
8. Under `Input Device`, select your external controller
9. Select your `Controller Type`
   - Select either `Joycon Pair` or `Pro Controller` depending on the game you are playing
10. Click `Load` to the right of `Controller Type`
11. Under `Motion`, check `Enable Motion Controls` and uncheck `Use CemuHook compatible motion`
12. Exit out of Ryujinx
13. Switch to `Game Mode`
14. In Game Mode, connect your controller
15. Select your Nintendo Switch game
16. On the `Play` screen, select the `Controller` icon to the right of the screen
    <img src="https://github.com/dragoonDorise/EmuDeck/assets/108900299/468d63e3-534c-4270-ac61-06e167d6df48" height="300">
17. Select your controller tab at the top
    <img src="https://github.com/dragoonDorise/EmuDeck/assets/108900299/b51a1405-9cdf-4ba3-bebf-db817f057f63" height="300">
18. Click the `Gear` icon to the right, and click `Disable Steam Input`
    <img src="https://github.com/dragoonDorise/EmuDeck/assets/108900299/33cbcb8e-a444-4a75-8e4a-ba9451e6e07a" height="300">
    - You may need to restart first for this setting to properly apply
19. Your controller's gyro will now work for this selected game, repeat as needed for your other games

If your controller gyro does not work after the above steps, reset Ryujinx's configuration in the EmuDeck application on the Manage Emulators page and try again.

#### Post-Configuration

To restore the default Steam Deck controls:

1. Open Ryujinx
2. Click `Options` at the top, click `Settings`
3. Click the `Input` tab on the top
4. Click `Configure` under `Player 1`
5. Select `Steam Virtual Gamepad` under `Input Device`
6. Click `Load` on the right side of the screen
7. Click `Save` and exit out of Ryujinx

(Optional) To restore Steam Input:

1. Select your Nintendo Switch game
2. On the `Play` screen, select the `Controller` icon to the right of the screen
   <img src="https://github.com/dragoonDorise/EmuDeck/assets/108900299/468d63e3-534c-4270-ac61-06e167d6df48" height="300">
3. Select your controller tab at the top
   <img src="https://github.com/dragoonDorise/EmuDeck/assets/108900299/b51a1405-9cdf-4ba3-bebf-db817f057f63" height="300">
4. Click the `Gear` icon to the right, and click `Enable Steam Input`
   - You may need to restart first for this setting to properly apply
5. The controls will be reverted to Steam Input and the Steam Deck controls will be restored

---

### How to Optimize Performance (Power Tools)



Visit [Power Tools](../../emudeck-application/steamos/emudeck-application-101.md#power-tools) to learn how to optimize performance using Power Tools.

---

### How to Configure Multiplayer



Ryujinx comes with a nifty auto-map feature that makes setting up multiplayer a breeze. To set up multiplayer, you simply need to enable the additional ports.

1. In **Game Mode**, open Ryujinx
   - You may add Ryujinx to Steam by using the `Emulators` parser in Steam ROM Manager
2. Open the `Input` settings in the `Settings` menu
3. For each controller you are using for Player 2, 3, 4, etc, click the respective `Configure` button
   - You do not need to adjust any settings for Player 1
4. Under `Input Device`
   - Player 2: `Steam Virtual Gamepad 1`
   - Player 3: `Steam Virtual Gamepad 2`
   - Player 4: `Steam Virtual Gamepad 3`
   - Player 5: `Steam Virtual Gamepad 4`
   - Player 6: `Steam Virtual Gamepad 5`
   - Player 7: `Steam Virtual Gamepad 6`
   - Player 8: `Steam Virtual Gamepad 7`
5. Using `Player 2` as an example:
   - On the `Player 2` configuration screen, after you have selected the appropriate `Input Device`, select your preferred `Controller Type` and click `Load` to the right of `Profile`
6. After you are finished enabling any additional players, click `Save` and you may open your game either directly as a shortcut in Steam or through ES-DE
7. (Optional) You may need to re-arrange the controller order in Game Mode for your controllers to function as expected. See [How to Re-Arrange the Controller Order](../../controls-and-hotkeys/steamos/external-controllers.md#how-to-re-arrange-the-controller-order) to learn how

---

### How to Install Mods



**Mod Resources**

_This list is not comprehensive_

- GameBanana Mods: [https://gamebanana.com/](https://gamebanana.com/)
  - Search by game name
- Nexus Mods: [https://www.nexusmods.com/](https://www.nexusmods.com/)
  - Search by game name
- GBAtemp: [https://gbatemp.net/forums/nintendo-switch.283/?prefix_id=56](https://gbatemp.net/forums/nintendo-switch.283/?prefix_id=56)
  - Use [https://gbatemp.net/search/?type=post](https://gbatemp.net/search/?type=post) to search
    - Sort by `ROM Hack` in the prefixes list and `Nintendo Switch` in the `Search in forums` list
  - To narrow search results, use the `Search titles only` toggle
- SweetFX: [http://sfx.thelazy.net/games/](http://sfx.thelazy.net/games/)
  - Search by game name
- theboy181
  - 1: Github Collection: [https://github.com/theboy181/switch-ptchtxt-mods](https://github.com/theboy181/switch-ptchtxt-mods)
  - 2: Github Collection: [https://github.com/theboy181/switch-cheat-mods](https://github.com/theboy181/switch-cheat-mods)
  - 3: theboy181's Discord: [https://linktr.ee/theboy181](https://linktr.ee/theboy181)

---

**Preface**

Read Ryujinx's instructions on how to install mods here: [How to Install Ryujinx Mods](https://github.com/Ryujinx/Ryujinx/wiki/Ryujinx-Setup-&-Configuration-Guide/87dc34d49facc69bb1b4fde45e1f10b520171671#managing-mods)

The folder structure of a mod is important. It should generally look like the following:

```
mod_directory
  - exefs
  - romfs
  - romfs_ext
```

---

**Tutorial**

1. In Desktop Mode, open Ryujinx
2. Right click a game you intend on modding
3. Click `Open Mod Data Location`
   1. <img src="https://user-images.githubusercontent.com/108900299/216734189-2a54fdcf-2720-41de-9dbd-3126f6ab4009.png" height="300">
4. Place your mod folder in the opened folder
   1. You may need to extract the mod first
   2. <img src="https://user-images.githubusercontent.com/108900299/216734205-c48b06a7-bfed-4e1c-9f3a-e02e9bac93e7.png" height="300">
5. Your mod is now installed

---

### Special Characters



Files with special characters in the ROM name will not launch from steam. Rename your ROMs and remove the special character.

Known **Cases**:

- `é` in `Pokémon`
- `'` in `The Legend of Zelda: Link's Awakening`
- `+` and `'` in `Super Mario 3D World + Bowser’s Fury`

If you used Steam ROM Manager previously, re-run Steam ROM Manager after renaming your ROMs.

**How to Remove Special Characters**

<figure class="video_container">
  <video controls="true" allowfullscreen="true">
    <source src="/videos/how-to-remove-special-characters.mp4" type="video/mp4">
  </video>
</figure>

---

### How to Roll Back Ryujinx to an Older Version



#### Preface


Your ROMs launch using a script created by EmuDeck, `ryujinx.sh` in `Emulation/tools/launchers`.

The script launches the corresponding emulator in `/home/deck/Applications/publish` and **specifically looks** for two traits:

- The most recently downloaded version of the emulator in `/home/deck/Applications/publish`, based on the file/release date.
- The emulator name at the beginning of the file. Anything after the emulator name is ignored.
  - For example, if the latest version of the emulator is `1351` and you would like to downgrade to `1349`. When you download version `1349`, you could rename it to `EMULATORNAME-1349.AppImage`, and EmuDeck's script will ignore the `-1349` in the file name, allowing you to record which versions of the emulator you are using through the file name.

#### How to Roll Back and Manually Install Ryujinx

* SteamOS and Linux


1. Download the version of the emulator you would like to use from GitLab: [https://git.ryujinx.app/ryubing/ryujinx/-/releases](https://git.ryujinx.app/ryubing/ryujinx/-/releases)
2. Move the downloaded emulator from Step 1 to `/home/deck/Applications/publish`
3. (Optional) Rename or delete the original emulator file if it exists.
4. Go into the EmuDeck app, Manage Emulators, Ryujinx, and hit "reset configuration" to obtain the correct configurations.

* Windows

1. Download the version of the emulator you would like to use from GitLab: [https://git.ryujinx.app/ryubing/ryujinx/-/releases](https://git.ryujinx.app/ryubing/ryujinx/-/releases)
2. Move the downloaded emulator and it's associated files to `Users/USERNAME/AppData/Roaming/EmuDeck/Emulators/Ryujinx`, if the Ryujinx folder does not exist, you can create it.
3. (Optional) Rename or delete the original emulator files if they exist.
4. Go into the EmuDeck app, Manage Emulators, Ryujinx, and hit "reset configuration" to obtain the correct configurations.


---

### How to Select Between Yuzu and Ryujinx in Game Mode



If you are using Steam ROM Manager and would like to run some games through Yuzu and others through Ryujinx, you may use Steam ROM Manager's exception manager to selectively run your games in your preferred emulator.

For further instructions, see [Steam ROM Manager: How to Hide ROMs on a Per Parser Basis](../../tools/steamos/steam-rom-manager.md#how-to-hide-roms-on-a-per-parser-basis).

If you are using ES-DE, you may use ES-DE's alternative emulators feature to select on a per-game basis which to run through Yuzu and which to run through Ryujinx.

For further instructions, see [ES-DE: How to Select a Different Emulator on a Per-Game Basis](../../tools/steamos/es-de.md#how-to-select-a-different-emulator-on-a-per-game-basis).

---

### How to Configure Language Settings



#### UI

1. In Desktop Mode, open Ryujinx
2. At the top, click `Options`, click `Change Language`
3. Select your preferred language in the menu

#### In-Game

1. In Desktop Mode, open Ryujinx
2. At the top, click `Options`, click `Settings`
3. Click the `System` tab
4. To the right of `System Language`, select your preferred language in the drop-down menu

---
