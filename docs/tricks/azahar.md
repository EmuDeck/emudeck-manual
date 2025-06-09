# <img src="/assets/emulators/azahar.png" alt="EmuDeck guide" width="80" style="vertical-align: middle"> Azahar Tips and Tricks

[TOC]

---

## Getting Started with Azahar
[Back to the Top](#azahar-tips-and-tricks)

Azahar is a fairly straight-forward emulator to set up. Place your ROMs in `Emulation/roms/n3ds` or `Emulation/roms/3ds`. Read the [Configuration](#azahar-configuration) section to learn more about Azahar and its folder locations. The [Configuration](#azahar-configuration).

To launch your ROMs in game mode, use Steam ROM Manager and use one of the following parsers to play your Azahar ROMs:

* `EmulationStation-DE`
* `Nintendo 3DS - Azahar` 
* `Emulators`


---

### Azahar Configuration
[Back to the Top](#azahar-tips-and-tricks)

* Type of Emulator: AppImage
* Config Location: 
    * `/home/deck/.config/azahar-emu`
    * `/home/deck/.local/share/azahar-emu`
* ROM Location: `Emulation/roms/3ds` or `Emulation/roms/n3ds`
* Saves Location:
    * Symlink: `Emulation/saves/azahar/saves`
    * Target: `/Emulation/storage/azahar/sdmc`
* Save States Location:
    * Symlink: `Emulation/saves/azahar/states/`
    * Target: `/home/deck/.local/share/azahar-emu/states`

**Note:** `~/.config` and `~/.local` are hidden folders by default. In Dolphin (file manager), click the hamburger menu in the top right, click `Show Hidden Files` to see these folders.

Azahar Works With:
* Steam ROM Manager
* ES-DE

---

### Azahar Folder Locations
[Back to the Top](#azahar-tips-and-tricks)

These file locations apply regardless of where you chose to install EmuDeck (to your internal SSD, to your SD Card, or elsewhere). Some emulator configuration files will be located on the internal SSD as listed below. 

`$HOME` refers to your home folder. If you are on a Steam Deck, this folder will be named `/home/deck` (you will likely not see `deck` in the file path when navigating using the file manager). 

Paths beginning with `Emulation/..` correspond to your EmuDeck install location. If you installed on an SD Card, your path may be `/run/media/mmcblk0p1/Emulation/roms/..`. If you installed on your internal SSD, your path may be `/home/deck/Emulation/roms/..`

**Note:** Folders with a `.` (`.var`, `.local`, `.config`, etc.) at the beginning are hidden by default. In Dolphin (file manager), click the hamburger menu in the top right, click `Show Hidden Files` to see these folders.

`/home/deck/.config/azahar-emu`

```
azahar-emu/
├── custom
├── qt-config.ini
└── qt-config.ini.bak
```

`/home/deck/.local/share/azahar-emu`

```
azahar-emu/
├── cheats
├── load
│   └── textures
├── log
│   ├── azahar_log.txt
│   └── azahar_log.txt.old.txt
├── shaders
│   └── vulkan
├── states
├── sysdata
│   └── mcu.dat
└── textures
```

`Emulation/storage/azahar`

```
azahar/
├── cheats -> /home/deck/.local/share/azahar-emu/cheats
├── nand
│   └── data
│       └── 00000000000000000000000000000000
│           ├── extdata
│           │   └── 00048000
│           └── sysdata
│               ├── 00010017
│               ├── 00010026
│               └── 00010035
├── screenshots
├── sdmc
│   └── Nintendo 3DS
│       └── 00000000000000000000000000000000
│           └── 00000000000000000000000000000000
│               └── title
└── textures -> /home/deck/.local/share/azahar-emu/load/textures
```


---

### How to Update Azahar
[Back to the Top](#azahar-tips-and-tricks)

**How to Update Azahar**

* Through the `Update your Emulators & Tools` section on the `Manage Emulators` page in the `EmuDeck` application
* Manual file replacement of `azahar-gui.AppImage` or `azahar.exe`.
    * AppImage can be replaced in `Home/Applications`, Windows executable and it's associated files can be replaced in `%APPDATA%/Roaming/EmuDeck/Emulators/Azahar`.
* Through the emulator GUI itself by launching the AppImage/Windows executable.


---

### How to Launch Azahar in Desktop Mode

**How to Launch Azahar in Desktop Mode**

* Launch `Azahar` from the Applications Launcher (Steam Deck icon in the bottom left of the taskbar or Windows icon)
* Launch the script from `Emulation/tools/launchers`, `azahar.sh` (SteamOS/Linux only)
* Launch the emulator from `Steam` after adding it via the `Emulators` parser in `Steam ROM Manager`


---

### Azahar File Formats
[Back to the Top](#azahar-tips-and-tricks)

* .cia
* .app 
* .axf 
* .cci 
* .cxi 
* .elf

**IMPORTANT:** 

* `.cia` can only be used if you install it through Azahar. **Do not** place your `.cia` ROMs in either the `Emulation/roms/3ds` or the `Emulation/roms/n3ds` folders. The .cia file format **is not** compatible with Steam ROM Manager and EmulationStation-DE.
* `.3ds` and `.3dsx` are no longer supported, you will have to change the file extension to `.cci` to use the file with Azahar.
* Encrypted ROMS are no longer supported, you must decrypt them or dump the games with GodMode9 in order to use them.
***

### How to Manage DLC and Updates
[Back to the Top](#azahar-tips-and-tricks)

DLC and update files typically are .CIAs, an installable file format through Azahar. These files need to be decrypted. After installing your DLC or updates, you may discard these files. 
If you have installed your system files and have your NNID sorted, you can also download your DLC/Updates from the Nintendo EShop.

**How to Install DLC and Updates**

1. In Desktop Mode, open Azahar
2. Click `File` in the top left 
3. Click `Install CIA...`
4. Navigate to your DLC or update files

---

### Azahar Hotkeys
[Back to the Top](#azahar-tips-and-tricks)

Azahar comes with a Steam Input profile for Hotkeys. When playing Azahar ROM shortcuts through Steam, the `EmuDeck - Controller Hotkeys` profile will automatically be applied so you may use the below hotkeys. For more info, see [Emulator Button Combinations Profile](../../controls-and-hotkeys/steamos/hotkeys.md#emulator-button-combinations-profile).

When using a frontend (ES-DE, Pegasus, or the emulator itself), the `EmuDeck - Frontend Controller Hotkeys` will automatically be applied. Hold `Start` for a few seconds to switch to the action set required to use the below hotkeys. For more info, see [Emulator Frontends Button Combinations Profile](../../controls-and-hotkeys/steamos/hotkeys.md#emulator-frontends-button-combinations-profile).

{{ read_csv('citra-hotkeys.csv') }}


**Note** 

* For a tutorial on how to select Steam Input Profiles, refer to: [How to Select a Steam Input Profile](../../controls-and-hotkeys/steamos/hotkeys.md#how-to-select-a-steam-input-profile).
* If you would like to use touch menus if your device supports it, apply the `EmuDeck - Steam Deck Radial Menus` profile instead.  
* [Steam Deck Button Layout](../../controls-and-hotkeys/steamos/hotkeys.md#steam-deck-button-layout)

---

## Azahar Common Issues
[Back to the Top](#azahar-tips-and-tricks)

---

### Why did my game suddenly stop working? 
[Back to the Top](#azahar-tips-and-tricks)

If your game ever crashes or you exit the game by pressing the `STEAM` button and clicking `Exit Game` instead of using the hotkey (`Quit` on the left trackpad), you may end up corrupting the shader cache. 

To clear the shader cache:

1. In Desktop Mode, open Azahar, File > Open Azahar Folder
2. Delete the `shaders` folder
3. Try your game again

**Note:** Use the `Select` + `Start` hotkey to exit your game instead of using the `STEAM` button. 

---

### How to Configure Gyro
[Back to the Top](#azahar-tips-and-tricks)

Gyro for Azahar requires SteamDeckGyroDSU. SteamDeckGyroDSU can be installed via EmuDeck, or it can be installed manually.

Visit [SteamDeckGyroDSU](../../emudeck-application/steamos/emudeck-application-101.md#steamdeckgyrodsu) to learn how to install and utilize SteamDeckGyroDSU. 

---

### How to Configure Gyro With External Controllers
[Back to the Top](#azahar-tips-and-tricks)

#### Desktop Mode

1. Switch to Desktop Mode
2. Exit out of Steam
    * You may exit out of Steam a couple of different ways:
        * Right click the `Steam` icon in your taskbar and click `Exit Steam`
        * Open Steam, click the `Steam` button in the top left, click `Exit`
        * Open a terminal (Konsole) and enter `killall -9 steam`
        * Do note that clicking the the `X` button in the top right of the Steam window **will not** exit out of Steam
    * Your controls will switch to `Lizard Mode`. Use `L2` to right click, `R2` to left click, and the `Right Trackpad` to move the mouse
    * You may also connect an external keyboard and mouse
2. Click the bluetooth icon in the bottom right of your taskbar and connect your controller
    * <img src="https://github.com/dragoonDorise/EmuDeck/assets/108900299/24945d4c-df06-4fbe-9668-7becea0c5edb" height="300">
3. Open Azahar
4. Click `Emulation` at the top, click `Configure`
5. Click `Controls` on the left
6. Click `New` to the right of `Profile` and give it a unique name
7. Click `Motion / Touch..` in the bottom left
8. To the right of `Motion Provider`, select `SDL` in the drop-down menu
9. Click `Configure` and follow the instructions
10. Click `OK`
11. Click `OK` again and exit out of Azahar
12. Switch to `Game Mode`

#### Game Mode/Big Picture Mode

1. In Game Mode, connect your controller
2. Select your Nintendo 3DS game 
3. On the `Play` screen, select the `Controller` icon to the right of the screen 
    * <img src="https://github.com/dragoonDorise/EmuDeck/assets/108900299/468d63e3-534c-4270-ac61-06e167d6df48" height="300">
4. Select your controller tab at the top
    * <img src="https://github.com/dragoonDorise/EmuDeck/assets/108900299/b51a1405-9cdf-4ba3-bebf-db817f057f63" height="300">
5. Click the `Gear` icon to the right, and click `Disable Steam Input`
    * <img src="https://github.com/dragoonDorise/EmuDeck/assets/108900299/33cbcb8e-a444-4a75-8e4a-ba9451e6e07a" height="300">
    * You may need to restart first for this setting to properly apply
6. Your controller's gyro will now work for this selected game, repeat as needed for your other games

#### Post-Configuration

To restore the default Steam Deck controls:

1. Open Azahar
2. Click `Emulation` at the top, click `Configure`
3. Click `Controls` on the left
4. To the right of `Profile`, select `SD-Default` in the drop-down menu
5. Click `OK` and exit out of Azahar

(Optional) To restore Steam Input:

1. Select your Nintendo 3DS game 
2. On the `Play` screen, select the `Controller` icon to the right of the screen 
    * <img src="https://github.com/dragoonDorise/EmuDeck/assets/108900299/468d63e3-534c-4270-ac61-06e167d6df48" height="300">
3. Select your controller tab at the top
    * <img src="https://github.com/dragoonDorise/EmuDeck/assets/108900299/b51a1405-9cdf-4ba3-bebf-db817f057f63" height="300">
4. Click the `Gear` icon to the right, and click `Enable Steam Input`
    * You may need to restart first for this setting to properly apply
5. The controls will be reverted to Steam Input and the Steam Deck controls will be restored

---

### How to Optimize Performance (Power Tools)
[Back to the Top](#azahar-tips-and-tricks)

Visit [Power Tools](../../emudeck-application/steamos/emudeck-application-101.md#power-tools) to learn how to optimize performance using Power Tools. 

---

### How to Install Custom Textures
[Back to the Top](#azahar-tips-and-tricks)

Here's how to install custom textures for Azahar:

Azahar Configuration

1. Open Azahar directly.
2. Click `Emulation` in the top left. Click `Configuration`, `Graphics`, and check both `Use Custom Textures` and `Async Custom Texture Loading`
    * <img src="https://user-images.githubusercontent.com/108900299/236593948-5a918187-27a7-4f5f-ac64-3b3147be8825.png" height="300">

**Note:** `Preload Custom Textures` is no longer recommended. Leave `Preload Custom Textures` off

How to Install Custom Textures

**Note:** Your texture pack may already come properly named and packaged with the correct `TitleID` and texture files. You may place the included texture pack folder directly into `/home/deck/.local/share/azahar-emu/textures/` or `%APPDATA%/Roaming/EmuDeck/Emulators/Azahar\user`. You do not need the following section if this is the case.

1. Open [https://3ds.jdbye.com/?details=USA&split=0&display=0](https://3ds.jdbye.com/?details=USA&split=0&display=0) in a browser.
2. Note down the `Title ID` for the game
    * For example, The Legend of Zelda: Majora's Mask 3D's (US) Title ID is: `0004000000125500` 
3. Open `/home/deck/.local/share/azahar-emu/textures/` or `%APPDATA%/Roaming/EmuDeck/Emulators/Azahar/user`
    * `~/.local` is a hidden folder by default. In Dolphin (file manager), click the hamburger menu in the top right, click `Show Hidden Files` to see these folders
4. In the `textures` folder from Step 3, create a folder matching the `TitleID` from Step 2
5. Put your texture files directly into the `TitleID` folder you created in Step 4
6. Your texture pack should now be installed

!!! tip
    
    Consider enabling `Preload Custom Textures`. This may help performance in some cases. 


---

### How to Use Cheats
[Back to the Top](#azahar-tips-and-tricks)


**Cheat Sources**

_This list is not exhaustive_

* [https://github.com/iSharingan/CTRPF-AR-CHEAT-CODES/tree/master/Cheats](https://github.com/iSharingan/CTRPF-AR-CHEAT-CODES/tree/master/Cheats)

#### How to Use Cheats

1. In Desktop Mode, open Azahar
2. Right click a game of your choice, click `Properties`
    * <img src="https://user-images.githubusercontent.com/108900299/236593492-91df7ce3-efae-4bb7-a559-7c252637a2e4.png" height="300">
3. Click the `Cheats` tab
    * <img src="https://user-images.githubusercontent.com/108900299/236593531-c045ab6e-3779-4c5a-b6ce-0af4a243f121.png" height="300">
4. Click `Add Cheat`
5. Name the cheat and add the code to the box under `Code:`
    * <img src="https://user-images.githubusercontent.com/108900299/236593755-85163908-cc80-4684-a343-01f180f14365.png" height="300">
6. Click Save in the top right
7. Check the box to the left of the cheat to enable it
    * <img src="https://user-images.githubusercontent.com/108900299/236593806-1f8973a4-cd67-4c35-b18e-14a5fbb30105.png" height="300"> 

---

### How to Roll Back Azahar to an Older Version
[Back to the Top](#azahar-tips-and-tricks)

The Appimage executable for Azahar is stored in `Home/Applications`, the Windows executable and it's associated files is stored in `%APPDATA%/Roaming/EmuDeck/Emulators/Azahar`, replace these files with the version you intend to use from the releases page: [https://github.com/azahar-emu/azahar/releases](https://github.com/azahar-emu/azahar/releases)

---

### How to Configure Language Settings
[Back to the Top](#azahar-tips-and-tricks)

#### UI

1. Open Azahar directly.
2. At the top, click `Emulation`, click `Configure`
3. On the left hand-side of the screen, click `General`
4. Click the `UI` tab
5. Under `General`, select your preferred language in the drop-down menu

#### In-Game

1. Open Azahar directly.
2. At the top, click `Emulation`, click `Configure`
3. On the left hand-side of the screen, click `System`
4. Click the `System` tab
5. Under `System Settings`, select your preferred language in the drop-down menu

---

## Custom Screen Layouts
[Back to the Top](#azahar-tips-and-tricks)

---

### How to Create Custom Screen Layouts.
[Back to the Top](#azahar-tips-and-tricks)

* (Instructions are SteamOS/Linux only)

Use [https://jesuscc1993.github.io/miscellaneous/citra-layout-generator/](https://jesuscc1993.github.io/miscellaneous/citra-layout-generator/) to create custom layouts.

After you have created your custom layout, use the following steps to use it. 

1. Open the folder: `/home/deck/.config/azahar-emu/`
    * `~/.config` is a hidden folder by default. In Dolphin (file manager), click the hamburger menu in the top right, click `Show Hidden Files` to see these folders
2. Right click `qt-config.ini`, and click `Open with Kate` or a text editor of your choice
3. Locate the `[Layout]` section
4. Replace the content of the `[Layout]` section with your newly created layout

---

### How to Configure Bottom Screen as PiP
[Back to the Top](#azahar-tips-and-tricks)

Credit: `NexLevel`

* (Instructions are SteamOS/Linux only)

Azahar allows you to configure the bottom screen as a sort of PiP (Picture in Picture) overlay on the top screen, by editing the qt-config file. 

**Here's How**

1. Open the folder: `/home/deck/.config/azahar-emu/`
    * `~/.config` is a hidden folder by default. In Dolphin (file manager), click the hamburger menu in the top right, click `Show Hidden Files` to see these folders
2. Right click `qt-config.ini`, and click `Open with Kate` or a text editor of your choice
3. Locate the `[Layout]` section
4. Replace the content of the `[Layout]` section with the below text:


        [Layout]
        anaglyph_shader_name=dubois (builtin)
        anaglyph_shader_name\default=true
        custom_bottom_bottom=800
        custom_bottom_bottom\default=false
        custom_bottom_left=520
        custom_bottom_left\default=false
        custom_bottom_right=760
        custom_bottom_right\default=false
        custom_bottom_top=620
        custom_bottom_top\default=false
        custom_layout=true
        custom_layout\default=false
        custom_second_layer_opacity=33
        custom_second_layer_opacity\default=false
        custom_top_bottom=784
        custom_top_bottom\default=false
        custom_top_left=0
        custom_top_left\default=true
        custom_top_right=1280
        custom_top_right\default=false
        custom_top_top=16
        custom_top_top\default=false
        factor_3d=0
        factor_3d\default=true
        filter_mode=true
        filter_mode\default=true
        large_screen_proportion=@Variant(\0\0\0\x87@\x80\0\0)
        large_screen_proportion\default=false
        layout_option=1
        layout_option\default=false
        mono_render_option=0
        mono_render_option\default=true
        pp_shader_name=none (builtin)
        pp_shader_name\default=true
        render_3d=0
        render_3d\default=true
        swap_screen=false
        swap_screen\default=true
        upright_screen=false
        upright_screen\default=true
                

5. (Optional) To move the PiP screen up, try setting `custom_top_top=0` and `custom_top_bottom=768`
6. Save and exit out of the text file, Azahar will now be using the bottom screen as PiP

**Note:** To revert back to defaults, the default `[Layout]` section is: 

```
[Layout]
anaglyph_shader_name=dubois (builtin)
anaglyph_shader_name\default=true
custom_bottom_bottom=480
custom_bottom_bottom\default=true
custom_bottom_left=40
custom_bottom_left\default=true
custom_bottom_right=360
custom_bottom_right\default=true
custom_bottom_top=240
custom_bottom_top\default=true
custom_layout=false
custom_layout\default=true
custom_second_layer_opacity=100
custom_second_layer_opacity\default=true
custom_top_bottom=240
custom_top_bottom\default=true
custom_top_left=0
custom_top_left\default=true
custom_top_right=400
custom_top_right\default=true
custom_top_top=0
custom_top_top\default=true
factor_3d=0
factor_3d\default=true
filter_mode=true
filter_mode\default=true
large_screen_proportion=@Variant(\0\0\0\x87@\x80\0\0)
large_screen_proportion\default=true
layout_option=2
layout_option\default=false
mono_render_option=0
mono_render_option\default=true
pp_shader_name=none (builtin)
pp_shader_name\default=true
render_3d=0
render_3d\default=true
swap_screen=false
swap_screen\default=true
upright_screen=false
upright_screen\default=true
```


---

### How to Configure Bottom Screen With PiP and Opacity
[Back to the Top](#azahar-tips-and-tricks)

Credit: `NexLevel`

* (Instructions are SteamOS/Linux only)

A previous update of Citra that Azahar has now used allows the ability to set the opacity on the bottom screen. In combination with setting the bottom screen as a PiP overlay, you can create a Azahar layout that looks like the following: 

**Example 1:** <img src="https://user-images.githubusercontent.com/108900299/219829080-3e871ada-cde0-44b5-9781-0294a9a9fc7b.png" height="300">

**Example 2:** <img src="https://user-images.githubusercontent.com/108900299/219829095-8fe0e1e9-aa15-4750-b917-899373ce10e7.png" height="300">
 
**Here's How**

1. Open the folder: `/home/deck/.config/azahar-emu/`
    * `~/.config` is a hidden folder by default. In Dolphin (file manager), click the hamburger menu in the top right, click `Show Hidden Files` to see these folders
2. Right click `qt-config.ini`, and click `Open with Kate` or a text editor of your choice
3. Locate the `[Layout]` section
4. Replace the content of the `[Layout]` section with the below text:

         
        [Layout]
        anaglyph_shader_name=dubois (builtin)
        anaglyph_shader_name\default=true
        custom_bottom_bottom=800
        custom_bottom_bottom\default=false
        custom_bottom_left=520
        custom_bottom_left\default=false
        custom_bottom_right=760
        custom_bottom_right\default=false
        custom_bottom_top=620
        custom_bottom_top\default=false
        custom_layout=true
        custom_layout\default=false
        custom_second_layer_opacity=33
        custom_second_layer_opacity\default=false
        custom_top_bottom=784
        custom_top_bottom\default=false
        custom_top_left=0
        custom_top_left\default=true
        custom_top_right=1280
        custom_top_right\default=false
        custom_top_top=16
        custom_top_top\default=false
        factor_3d=0
        factor_3d\default=true
        filter_mode=true
        filter_mode\default=true
        large_screen_proportion=@Variant(\0\0\0\x87@\x80\0\0)
        large_screen_proportion\default=false
        layout_option=1
        layout_option\default=false
        mono_render_option=0
        mono_render_option\default=true
        pp_shader_name=none (builtin)
        pp_shader_name\default=true
        render_3d=0
        render_3d\default=true
        swap_screen=false
        swap_screen\default=true
        upright_screen=false
        upright_screen\default=true
         

5. To adjust the PiP opacity, the opacity can be any integer between 1-100
6. Save and exit out of the text file, Azahar will now be using the bottom screen as PiP with custom opacity

**Note:** To revert back to defaults, the default `[Layout]` section is: 

```
[Layout]
anaglyph_shader_name=dubois (builtin)
anaglyph_shader_name\default=true
custom_bottom_bottom=480
custom_bottom_bottom\default=true
custom_bottom_left=40
custom_bottom_left\default=true
custom_bottom_right=360
custom_bottom_right\default=true
custom_bottom_top=240
custom_bottom_top\default=true
custom_layout=false
custom_layout\default=true
custom_second_layer_opacity=100
custom_second_layer_opacity\default=true
custom_top_bottom=240
custom_top_bottom\default=true
custom_top_left=0
custom_top_left\default=true
custom_top_right=400
custom_top_right\default=true
custom_top_top=0
custom_top_top\default=true
factor_3d=0
factor_3d\default=true
filter_mode=true
filter_mode\default=true
large_screen_proportion=@Variant(\0\0\0\x87@\x80\0\0)
large_screen_proportion\default=true
layout_option=2
layout_option\default=false
mono_render_option=0
mono_render_option\default=true
pp_shader_name=none (builtin)
pp_shader_name\default=true
render_3d=0
render_3d\default=true
swap_screen=false
swap_screen\default=true
upright_screen=false
upright_screen\default=true
```

---

### How to Configure Bottom Screen as PiP in the Top Right Corner
[Back to the Top](#azahar-tips-and-tricks)

Picture: 

![How to Configure Bottom Screen as PiP in the Top Right Corner](../../assets/how-to-configure-bottom-screen-as-pip-in-the-top-right-corner.png)

Credit: `busywait`

* (Instructions are SteamOS/Linux only)

1. Open the folder: `/home/deck/.config/azahar-emu/`
    * `~/.config` is a hidden folder by default. In Dolphin (file manager), click the hamburger menu in the top right, click `Show Hidden Files` to see these folders
2. Right click `qt-config.ini`, and click `Open with Kate` or a text editor of your choice
3. Locate the `[Layout]` section
4. Replace the content of the `[Layout]` section with the below text:

         
        [Layout]
        anaglyph_shader_name=dubois (builtin)
        anaglyph_shader_name\default=true
        custom_bottom_bottom=240
        custom_bottom_bottom\default=false
        custom_bottom_left=960
        custom_bottom_left\default=false
        custom_bottom_right=1280
        custom_bottom_right\default=false
        custom_bottom_top=0
        custom_bottom_top\default=false
        custom_layout=true
        custom_layout\default=false
        custom_second_layer_opacity=80
        custom_second_layer_opacity\default=false
        custom_top_bottom=800
        custom_top_bottom\default=false
        custom_top_left=0
        custom_top_left\default=true
        custom_top_right=1200
        custom_top_right\default=false
        custom_top_top=80
        custom_top_top\default=false
        factor_3d=0
        factor_3d\default=true
        filter_mode=true
        filter_mode\default=true
        large_screen_proportion=4
        large_screen_proportion\default=true
        layout_option=1
        layout_option\default=false
        mono_render_option=0
        mono_render_option\default=true
        pp_shader_name=none (builtin)
        pp_shader_name\default=true
        render_3d=0
        render_3d\default=true
        swap_screen=false
        swap_screen\default=true
        upright_screen=false
        upright_screen\default=true
         
5. Save and close out of the text file
6. Azahar will now apply your custom layout

**Note:** To revert back to defaults, the default `[Layout]` section is: 

```
[Layout]
anaglyph_shader_name=dubois (builtin)
anaglyph_shader_name\default=true
custom_bottom_bottom=480
custom_bottom_bottom\default=true
custom_bottom_left=40
custom_bottom_left\default=true
custom_bottom_right=360
custom_bottom_right\default=true
custom_bottom_top=240
custom_bottom_top\default=true
custom_layout=false
custom_layout\default=true
custom_second_layer_opacity=100
custom_second_layer_opacity\default=true
custom_top_bottom=240
custom_top_bottom\default=true
custom_top_left=0
custom_top_left\default=true
custom_top_right=400
custom_top_right\default=true
custom_top_top=0
custom_top_top\default=true
factor_3d=0
factor_3d\default=true
filter_mode=true
filter_mode\default=true
large_screen_proportion=@Variant(\0\0\0\x87@\x80\0\0)
large_screen_proportion\default=true
layout_option=2
layout_option\default=false
mono_render_option=0
mono_render_option\default=true
pp_shader_name=none (builtin)
pp_shader_name\default=true
render_3d=0
render_3d\default=true
swap_screen=false
swap_screen\default=true
upright_screen=false
upright_screen\default=true
```

## Online Features

---
### How to Set Up System Files
[Back to the Top](#azahar-tips-and-tricks)

* Do NOT share any files obtained with these steps, as it could get your system banned from Nintendo or Pretendo servers.
* Make sure you have your Nintendo 3DS, as this process requires it.
* To install New 3DS system software, you need to download Old 3DS software first, this is required for some situations (such as Pretendo Network), so it's best to download both.
* The system used does not matter in this instance, you can download New 3DS software with an old 3DS, and vice versa.


1. Take out your SD Card and plug it into your PC.

2. Download the Azahar Setup Tool from the respective GitHub page, and place it in your cia or 3ds folder on the SD card. [https://github.com/azahar-emu/ArticSetupTool/releases](https://github.com/azahar-emu/ArticSetupTool/releases)

3. Insert your SD Card back into the Nintendo 3DS and power it on, launch the Setup Tool, instructions will vary depending on your chosen file.

 If you used the .3dsx, you need to launch it via the Homebrew Launcher.
 
 If you used the .cia, you need to install it with FBI.

4. Press A to start the setup tool, you will be given a local IP address once completed.

5. Launch Azahar, then File > Setup System Files, you will be prompted for a local IP address, type in the address displayed on the 3DS, and press OK.

6. You will be taken to the System Update screen if everything was done correctly, follow the prompts and wait for it to update.

7. Once successfully updated, confirm the update.

You should now have your system files ready to go.


---

### How to Set Up your Nintendo Network ID
[Back to the Top](#azahar-tips-and-tricks)

* Do note this process may make you unable to access certain features of Pretendo Network, such as Miiverse.
* This process requires atleast Old 3DS system software files, if you have not already done so, you can do so with the instructions in the [How To Set Up System Files](#how-to-set-up-system-files) section.


1. Download ThreeSD from the respective GitHub page and for your OS: [https://github.com/zhaowenlan1779/threeSD/releases](https://github.com/zhaowenlan1779/threeSD/releases)

2. Insert your 3DS SD Card into your computer and in the dist folder of the ThreeSD zip, copy the threeSDDumper.gm9 into your gm9/scripts folder on your SD Card. Eject the SD Card and put it back into your Nintendo 3DS.

3. Launch GodMode9 by holding the Start button then powering the Nintendo 3DS on.

4. Press the Home Button, Scripts, and then execute the threeSDDumper script. Once it is done, power off your 3DS and put the SD Card back into your PC and launch the threeSD executable.

5. After that click your SD card, uncheck everything but Ungrouped, and transfer the data.

* This data gets saved to the CITRA user save directory, not Azahar, so you need to locate this directory.

* for SteamOS and most Linux distros, it's located in `Home/.local/share`, but you can also locate it by launching Azahar and going to File > Open Azahar Folder, then go back one folder.
  
* Check where your SDMC folder is located, usually, they will be located in Azahar's folder, move the two newly created folders into that same directory displayed in Emulation > Configure > System > Storage.

6. Next, you need to link your NNID, make sure you have your ID, password, and email ready.

7. Launch Azahar, go into Emulation > Configure, then the System tab, and enable required LLE modules for online features.

8. Boot the Home Menu by going to File > Boot Home Menu > (Region of your Nintendo 3DS).
   
9.  Launch the System Settings app, Nintendo Network ID Settings, then follow the prompts until you are at the screen that either says `Existing ID` Or `Create New ID`, you want to hit the `Existing ID` button.

10. Type in your ID, Password, and email associated with the NNID.

After following the prompts, you should now have access to the Nintendo EShop or Pokémon Bank.


---
### How to Set Up Pretendo Network
[Back to the Top](#azahar-tips-and-tricks)

* This process requires both the old and New 3DS system software files, if you have not already done so, you can do so with the instructions in the [How To Set Up System Files](#how-to-set-up-system-files) section.
* Do note that if you have a NNID installed for usage of Pokémon Bank or the Nintendo EShop, you may not be able to use features that require an ID via Pretendo Network, which right now, is only Miiverse.


1. Download the .cia version of Nimbus from the respective GitHub page. [https://github.com/PretendoNetwork/nimbus/releases](https://github.com/PretendoNetwork/nimbus/releases)

2. Launch Azahar, go to File > Open Azahar Folder, and move both the luma and 3ds folder into the sdmc folder.

3. Back to Azahar, go to File > Install CIA, select the Nimbus.cia file, and it should now be installed.

4. Go to Emulation > Configure, then the System tab, you need to enable the required LLE modules for online features, this should be at the top of the System Settings section.

5. Afterwards, boot into the home menu by going to File > Boot Home Menu > (Region of your Nintendo 3DS).

6. Run the newly installed Nimbus program, and select Pretendo, it should take you back to the Home Menu.

You should now have access to the Pretendo Network.
 
---
