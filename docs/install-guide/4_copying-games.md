# :material-usb-port: Copying ROMS and BIOS

Wether you picked _Easy Mode_ or _Custom Mode_ you'll see this screen asking how you want to add your games

<img src="/assets/install_guide/copy-games.png" alt="EmuDeck guide">

!!! question "Which option should I pick?"

    === "Manual copy"
        By selecting this option EmuDeck will open your Emulation Folder so you can manually copy your ROMS and BIOS, make sure you copy each game to its appropiate folder.

        ??? info "BIOS folders explanation"

            Some systems need BIOS or firmware to work, you need to extract them from your system and place them in the following locations **without creating any additional subfolder**:

            | System                          | Location       |
            | ------------- | ----------- |
            | Playstation 1 | ==Emulation/bios== |
            | Playstation 2 | ==Emulation/bios== |
            | Playstation 3 | ==Must be installed using RPCS3== |
            | Nintendo Switch - Yuzu | ==Emulation/bios/yuzu/== |
            | Nintendo Switch - Ryujinx | ==Emulation/bios/Ryujinx/keys & firmware must be installed using Ryujinx== |
            | Nintendo Switch - Citron | ==Emulation/bios/citron== |
            | Nintendo DS | ==Emulation/bios== |
            | Sega Dreamcast | ==Emulation/bios/dc== |
            | Xbox | ==Emulation/bios== |

        ??? info "ROMS folders explanation"

            Each folder correlates to a system you can emulate.

            | Subfolder      | System                          |
            | ----------- | ------------------------------------ |
            | `3do` | Panasonic 3DO |
            |` ags` | Amiga AGS |
            | `amiga` | Amiga |
            |` amiga600` | Amiga 600 |
            | `amiga1200` | Amiga 1200 |
            |` amigacd32` | Amiga CD |
            | `amstradcpc` | Amstrad CPC |
            |` android` | **No emulator available yet** |
            | `apple2` | Apple 2 |
            |` apple2gs` | Apple 2 GS |
            | `arcade` | Mame |
            |` arcadia` | **No emulator available yet**  |
            | `arduboy` | **No emulator available yet**  |
            |` astrocde` | **No emulator available yet**  |
            | `atari800` | Atari 800 |
            |` atari2600` | Atari 2600 |
            | `atari5200` | Atari 5200 |
            |` atari7800` | Atari 7800 |
            | `atarijaguar` | Atari Jaguar |
            |` atarijaguarcd` | Atari Jaguar CD |
            | `atarilynx` | Atari Lynx |
            |` atarist` | Atari ST |
            | `atarixe` | Atari XE |
            |` atomiswave` | Sammy Atomiswave |
            | `bbcmicro` | **No emulator available yet**  |
            |` c16` | Commodore 16 |
            | `c64` | Commodore 64 |
            |` cavestory` | Cave Story |
            | `cdimono1` | Philips CD-i |
            |` cdtv` | Commodore CDTV |
            | `chailove` | ChaiLove Game Engine |
            |` channelf` | Fairchild Channel F |
            | `cloud` | Used for Cloud Services |
            |` coco` | Tandy Color Computer |
            | `colecovision` | ColecoVision |
            |` cps` | Capcom Play System |
            | `cps1` | Capcom Play System I |
            |` cps2` | Capcom Play System II |
            | `cps3` | Capcom Play System III |
            |` crvision` | VTech CreatiVision |
            | `daphne` | Daphne Arcade LaserDisc |
            |` desktop` | Remote Play Clients |
            | `doom` | DooM |
            |` dos` | MSDOS |
            | `dragon32` | Dragon 32 |
            |` dreamcast` | Dreamcast |
            | `easyrpg` | EasyRPG Game Engine |
            |` emulators` | Emulators links for ESDE |
            | `epic` | **Not used** |
            |` famicom` | Nintendo Family Computer |
            | `fba` | FinalBurn Alpha |
            |` fbneo` | FinalBurn Neo |
            | `fds` | Nintendo Famicom Disk System |
            |` flash` | Adobe Flash |
            | `fmtowns` | Fujitsu FM Towns |
            |` gameandwatch` | Nintendo Game and Watch |
            | `gamecom` | Tiger Electronics Game.com |
            |` gamegear` | Sega Game Gear |
            | `gb` | Nintendo Game Boy |
            |` gba` | Nintendo Game Boy Advance |
            | `gbc` | Nintendo Game Boy Color |
            |` gc` | Nintendo GameCube |
            | `generic-applications` | **Not used** |
            |` genesis` | Sega Genesis |
            | `genesiswide` | Sega Genesis WideScreen hacks |
            |` gx4000` | Amstrad GX4000 |
            | `intellivision` | Mattel Electronics Intellivision |
            |` j2me` | Java 2 Micro Edition (J2ME) |
            | `kodi` | **Not used** |
            |` lcdgames` | LCD Handheld Games |
            | `lutris` | **Not used**  |
            |` lutro` | Lutro Game Engine |
            | `macintosh` | Apple Macintosh |
            |` mame` | Multiple Arcade Machine Emulator |
            | `mame-advmame` | **Not used** |
            |` mame-mame4all` | **Not used** |
            | `mastersystem` | Sega Master System |
            |` megacd` | Sega MegaCD |
            | `megacdjp` | **Not used** |
            |` megadrive` | Sega MegaDrive |
            | `megadrivejp` | **Not used** |
            |` megaduck` | Creatronic Mega Duck |
            | `mess` | **Not used** |
            |` model2` | Sega Model 2 |
            | `model3` | Sega Model 3 |
            |`moonlight` | **Not used** |
            |`moto` | Thomson MO/TO Series |
            |`msx` | MSX |
            |`msx1` | MSX1 |
            |`msx2` | MSX2 |
            |`msxturbor` | MSX Turbo R |
            |`mugen` | M, U, G, E, N Game Engine -  **No emulator available yet** |
            |`multivision` | Othello Multivision |
            |`n3ds` | Nintendo 3DS |
            |`n64` | Nintendo 64 |
            |`n64dd` | Nintendo 64DD |
            |`naomi` | Sega NAOMI |
            |`naomi2` | Sega NAOMI 2 |
            |`naomigd` | Sega NAOMI GD-ROM |
            |`nds` | Nintendo DS |
            |`neogeo` | SNK Neo Geo |
            |`neogeocd` | SNK Neo Geo CD |
            |`neogeocdjp` | SNK Neo Geo CD - Japan |
            |`nes` | Nintendo Entertainment System |
            |`ngp` | SNK Neo Geo Pocket |
            |`ngpc` |  SNK Neo Geo Pocket Color |
            |`odyssey2` | Magnavox Odyssey2 |
            |`openbor` | OpenBOR Game Engine |
            |`oric` | Tangerine Computer Systems Oric |
            |`palm` | Palm OS |
            |`pc` | IBM PC |
            |`pc88` | NEC PC-8800 Series |
            |`pc98` | NEC PC-9800 Series |
            |`pcengine` | NEC PC Engine |
            |`pcenginecd` | NEC PC Engine CD |
            |`pcfx` | NEC PC-FX |
            |`pico8` | PICO-8 Fantasy Console |
            |`pokemini` | Nintendo Pokémon Mini |
            |`ports` | **Not used** |
            |`primehacks` | PrimeHack |
            |`ps2` | Sony PlayStation 2 |
            |`ps3` | Sony PlayStation 3 |
            |`ps4` | Sony PlayStation 4 |
            |`psp` | Sony PlayStation Portable |
            |`psvita` | Sony PlayStation Vita |
            |`psx` | Sony PlayStation |
            |`pv1000` | **No emulator available yet** |
            |`quake` | Quake |
            |`remoteplay` | Remote Play Clients |
            |`samcoupe` | SAM Coupé |
            |`satellaview` | Nintendo Satellaview |
            |`saturn` | Sega Saturn |
            |`saturnjp` | **Not used** |
            |`scummvm` | ScummVM Game Engine |
            |`sega32x` | Sega 32X |
            |`sega32xjp` | **Not used** |
            |`sega32xna` | **Not used** |
            |`segacd` | Sega CD |
            |`sfc` | Nintendo SFC (Super Famicom) |
            |`sg-1000` | Sega SG-1000 |
            |`sgb` | Nintendo Super Game Boy |
            |`snes` | Super Nintendo Entertainment System |
            |`sneshd` | Super Nintendo Entertainment System - Widescreen hacks |
            |`snesna` | **Not used**  |
            |`solarus` | Solarus Game Engine |
            |`spectravideo` | Spectravideo |
            |`steam` | **Not used**  |
            |`stratagus` | Stratagus Game Engine |
            |`sufami` | Bandai SuFami Turbo |
            |`supergrafx` | NEC SuperGrafx |
            |`supervision` | Watara Supervision |
            |`switch` | Nintendo Switch |
            |`symbian` | **Not used**  |
            |`tanodragon` | Tano Dragon |
            |`tg-cd` | NEC TurboGrafx-CD |
            |`tg16` | NEC TurboGrafx-16 |
            |`ti99` | Texas Instruments TI-99 |
            |`tic80` | TIC-80 Game Engine |
            |`to8` | Thomson TO8 |
            |`trs-80` | Tandy TRS-80 |
            |`uzebox` | Uzebox |
            |`vectrex` | Vectrex |
            |`vic20` | Commodore VIC-20 |
            |`videopac` | Philips Videopac G7000 |
            |`virtualboy` | Nintendo Virtual Boy |
            |`vsmile` | VTech V.Smile |
            |`wasm4` | WASM-4 Fantasy Console |
            |`wii` | Nintendo Wii |
            |`wiiu` | Nintendo Wii U |
            |`wonderswan` | Bandai WonderSwan |
            |`wonderswancolor` | Bandai WonderSwan Color |
            |`x1` | Sharp X1 |
            |`x68000` | Sharp X68000 |
            |`xbox` | Microsoft Xbox |
            |`xbox360` | Microsoft Xbox 360 |
            |`zmachine` | Infocom Z-machine - **No emulator available yet** |
            |`zx81` | Sinclair ZX81 |
            |`zxspectrum` | Sinclair ZX Spectrum |



    === "Automatic Import"

        !!! danger "This is only available for SteamOS/Linux"

        <img src="/assets/install_guide/copy-games-auto.png" alt="EmuDeck guide">
        This option will allow you to easily copy your ROMS and BIOS using an USB.

        **Instructions**

        - Insert a USB Drive in your system, click on *Select your USB Drive* and pick it on the selection menu. This will create a ==roms== and a ==bios== folder in your USB drive.
        - Leave the EmuDeck App open and eject your USB Drive, plug it into your computer and copy each game to its appropiate folder. If you have problems identifying which folder corresponds to each system read the "Rom folders explanation" down below

        ??? info "BIOS folders explanation"

            Some systems need BIOS or firmware to work, you need to extract them from your system and place them in the following locations **without creating any additional subfolder**:

            | System                          | Location       |
            | ------------- | ----------- |
            | Playstation 1 | ==Emulation/bios== |
            | Playstation 2 | ==Emulation/bios== |
            | Playstation 3 | ==Must be installed using RPCS3== |
            | Nintendo Switch - Yuzu | ==Emulation/bios/yuzu/== |
            | Nintendo Switch - Ryujinx | ==Emulation/bios/Ryujinx/keys & firmware must be installed using Ryujinx== |
            | Nintendo Switch - Citron | ==Emulation/bios/citron== |
            | Sega Dreamcast | ==Emulation/bios/dc== |
            | Nintendo DS | ==Emulation/bios== |



        ??? info "ROMS folders explanation"

            Each folder correlates to a system you can emulate.

            | Subfolder      | System                          |
            | ----------- | ------------------------------------ |
            | `3do` | Panasonic 3DO |
            |` ags` | Amiga AGS |
            | `amiga` | Amiga |
            |` amiga600` | Amiga 600 |
            | `amiga1200` | Amiga 1200 |
            |` amigacd32` | Amiga CD |
            | `amstradcpc` | Amstrad CPC |
            |` android` | **No emulator available yet** |
            | `apple2` | Apple 2 |
            |` apple2gs` | Apple 2 GS |
            | `arcade` | Mame |
            |` arcadia` | **No emulator available yet**  |
            | `arduboy` | **No emulator available yet**  |
            |` astrocde` | **No emulator available yet**  |
            | `atari800` | Atari 800 |
            |` atari2600` | Atari 2600 |
            | `atari5200` | Atari 5200 |
            |` atari7800` | Atari 7800 |
            | `atarijaguar` | Atari Jaguar |
            |` atarijaguarcd` | Atari Jaguar CD |
            | `atarilynx` | Atari Lynx |
            |` atarist` | Atari ST |
            | `atarixe` | Atari XE |
            |` atomiswave` | Sammy Atomiswave |
            | `bbcmicro` | **No emulator available yet**  |
            |` c16` | Commodore 16 |
            | `c64` | Commodore 64 |
            |` cavestory` | Cave Story |
            | `cdimono1` | Philips CD-i |
            |` cdtv` | Commodore CDTV |
            | `chailove` | ChaiLove Game Engine |
            |` channelf` | Fairchild Channel F |
            | `cloud` | Used for Cloud Services |
            |` coco` | Tandy Color Computer |
            | `colecovision` | ColecoVision |
            |` cps` | Capcom Play System |
            | `cps1` | Capcom Play System I |
            |` cps2` | Capcom Play System II |
            | `cps3` | Capcom Play System III |
            |` crvision` | VTech CreatiVision |
            | `daphne` | Daphne Arcade LaserDisc |
            |` desktop` | Remote Play Clients |
            | `doom` | DooM |
            |` dos` | MSDOS |
            | `dragon32` | Dragon 32 |
            |` dreamcast` | Dreamcast |
            | `easyrpg` | EasyRPG Game Engine |
            |` emulators` | Emulators links for ESDE |
            | `epic` | **Not used** |
            |` famicom` | Nintendo Family Computer |
            | `fba` | FinalBurn Alpha |
            |` fbneo` | FinalBurn Neo |
            | `fds` | Nintendo Famicom Disk System |
            |` flash` | Adobe Flash |
            | `fmtowns` | Fujitsu FM Towns |
            |` gameandwatch` | Nintendo Game and Watch |
            | `gamecom` | Tiger Electronics Game.com |
            |` gamegear` | Sega Game Gear |
            | `gb` | Nintendo Game Boy |
            |` gba` | Nintendo Game Boy Advance |
            | `gbc` | Nintendo Game Boy Color |
            |` gc` | Nintendo GameCube |
            | `generic-applications` | **Not used** |
            |` genesis` | Sega Genesis |
            | `genesiswide` | Sega Genesis WideScreen hacks |
            |` gx4000` | Amstrad GX4000 |
            | `intellivision` | Mattel Electronics Intellivision |
            |` j2me` | Java 2 Micro Edition (J2ME) |
            | `kodi` | **Not used** |
            |` lcdgames` | LCD Handheld Games |
            | `lutris` | **Not used**  |
            |` lutro` | Lutro Game Engine |
            | `macintosh` | Apple Macintosh |
            |` mame` | Multiple Arcade Machine Emulator |
            | `mame-advmame` | **Not used** |
            |` mame-mame4all` | **Not used** |
            | `mastersystem` | Sega Master System |
            |` megacd` | Sega MegaCD |
            | `megacdjp` | **Not used** |
            |` megadrive` | Sega MegaDrive |
            | `megadrivejp` | **Not used** |
            |` megaduck` | Creatronic Mega Duck |
            | `mess` | **Not used** |
            |` model2` | Sega Model 2 |
            | `model3` | Sega Model 3 |
            |`moonlight` | **Not used** |
            |`moto` | Thomson MO/TO Series |
            |`msx` | MSX |
            |`msx1` | MSX1 |
            |`msx2` | MSX2 |
            |`msxturbor` | MSX Turbo R |
            |`mugen` | M, U, G, E, N Game Engine -  **No emulator available yet** |
            |`multivision` | Othello Multivision |
            |`n3ds` | Nintendo 3DS |
            |`n64` | Nintendo 64 |
            |`n64dd` | Nintendo 64DD |
            |`naomi` | Sega NAOMI |
            |`naomi2` | Sega NAOMI 2 |
            |`naomigd` | Sega NAOMI GD-ROM |
            |`nds` | Nintendo DS |
            |`neogeo` | SNK Neo Geo |
            |`neogeocd` | SNK Neo Geo CD |
            |`neogeocdjp` | SNK Neo Geo CD - Japan |
            |`nes` | Nintendo Entertainment System |
            |`ngp` | SNK Neo Geo Pocket |
            |`ngpc` |  SNK Neo Geo Pocket Color |
            |`odyssey2` | Magnavox Odyssey2 |
            |`openbor` | OpenBOR Game Engine |
            |`oric` | Tangerine Computer Systems Oric |
            |`palm` | Palm OS |
            |`pc` | IBM PC |
            |`pc88` | NEC PC-8800 Series |
            |`pc98` | NEC PC-9800 Series |
            |`pcengine` | NEC PC Engine |
            |`pcenginecd` | NEC PC Engine CD |
            |`pcfx` | NEC PC-FX |
            |`pico8` | PICO-8 Fantasy Console |
            |`pokemini` | Nintendo Pokémon Mini |
            |`ports` | **Not used** |
            |`primehacks` | PrimeHack |
            |`ps2` | Sony PlayStation 2 |
            |`ps3` | Sony PlayStation 3 |
            |`ps4` | Sony PlayStation 4 |
            |`psp` | Sony PlayStation Portable |
            |`psvita` | Sony PlayStation Vita |
            |`psx` | Sony PlayStation |
            |`pv1000` | **No emulator available yet** |
            |`quake` | Quake |
            |`remoteplay` | Remote Play Clients |
            |`samcoupe` | SAM Coupé |
            |`satellaview` | Nintendo Satellaview |
            |`saturn` | Sega Saturn |
            |`saturnjp` | **Not used** |
            |`scummvm` | ScummVM Game Engine |
            |`sega32x` | Sega 32X |
            |`sega32xjp` | **Not used** |
            |`sega32xna` | **Not used** |
            |`segacd` | Sega CD |
            |`sfc` | Nintendo SFC (Super Famicom) |
            |`sg-1000` | Sega SG-1000 |
            |`sgb` | Nintendo Super Game Boy |
            |`snes` | Super Nintendo Entertainment System |
            |`sneshd` | Super Nintendo Entertainment System - Widescreen hacks |
            |`snesna` | **Not used**  |
            |`solarus` | Solarus Game Engine |
            |`spectravideo` | Spectravideo |
            |`steam` | **Not used**  |
            |`stratagus` | Stratagus Game Engine |
            |`sufami` | Bandai SuFami Turbo |
            |`supergrafx` | NEC SuperGrafx |
            |`supervision` | Watara Supervision |
            |`switch` | Nintendo Switch |
            |`symbian` | **Not used**  |
            |`tanodragon` | Tano Dragon |
            |`tg-cd` | NEC TurboGrafx-CD |
            |`tg16` | NEC TurboGrafx-16 |
            |`ti99` | Texas Instruments TI-99 |
            |`tic80` | TIC-80 Game Engine |
            |`to8` | Thomson TO8 |
            |`trs-80` | Tandy TRS-80 |
            |`uzebox` | Uzebox |
            |`vectrex` | Vectrex |
            |`vic20` | Commodore VIC-20 |
            |`videopac` | Philips Videopac G7000 |
            |`virtualboy` | Nintendo Virtual Boy |
            |`vsmile` | VTech V.Smile |
            |`wasm4` | WASM-4 Fantasy Console |
            |`wii` | Nintendo Wii |
            |`wiiu` | Nintendo Wii U |
            |`wonderswan` | Bandai WonderSwan |
            |`wonderswancolor` | Bandai WonderSwan Color |
            |`x1` | Sharp X1 |
            |`x68000` | Sharp X68000 |
            |`xbox` | Microsoft Xbox |
            |`xbox360` | Microsoft Xbox 360 |
            |`zmachine` | Infocom Z-machine - **No emulator available yet** |
            |`zx81` | Sinclair ZX81 |
            |`zxspectrum` | Sinclair ZX Spectrum |

        - Insert the USB Drive back to your system and go back to the EmuDeck App and click on the ==Button== to start and wait till all ROMS and BIOS are copied to your system.
