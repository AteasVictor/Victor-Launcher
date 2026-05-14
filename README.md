# Victor Launcher

Victor Launcher is an in-game mod manager for Among Us built on BepInEx.

It is designed to make DLL-based mod packs easier to manage without constantly dragging files in and out of the game folder by hand, and add effortless mod sharing through codes.

## Features

- open the launcher in game with F7
- install DLL mods from a simple in-game menu
- view installed, disabled, and queued mods
- enable or disable mods without manually sorting files
- manage grouped mod folders from one place
- download shared packs by room code and queue them for install

## Installation

1. Download the latest release asset.
2. Place the latest version of Victor Launcher into:

<Among Us folder>/BepInEx/plugins/, and the mod does the rest

3. Launch Among Us
4. Press F7 to open Victor Launcher

## How It Works

Just press "Upload Mod", and choose the plugin to install. The selected plugin will be queued.
Once installed, changes will take effect on the next restart. 
After a change affecting the mod is made, it will prompt you to close the game.

Victor Launcher keeps track of

- active plugins in `BepInEx/plugins`
- disabled plugins in `BepInEx/plugins-disabled`
- queued imports in `BepInEx/mod-imports`

Changes that affect loaded mods still require a game restart to fully take effect.

## Shared Packs

Victor Launcher supports room-code pack downloads.

To make the room:
1. visit the website at https://ateasvictor.github.io/Victor-Launcher/
2. create a room with a name, room code, and password (don't forget this)
3. upload your DLL's to the website (this creates a draft)
4. press 'save room pack' to upload the changes to the cloud
5. share the room code with your players 

If a host shares a valid room code, players can:

1. open Victor Launcher
2. enter the room code
3. download the pack into the queue
4. install the queued DLLs
5. restart the game when prompted

## Skins
- Victor launcher now supports skins in the .vsk format in versions 0.2.3 and newer.
- You can find a sample in the release of 0.2.3
- Just put the VSK file in the plugins folder alongside Victor Launcher and it will automatically use the skin.
- The skins allow you to customize the Header, button colors, and primary and secondary colors.

## Notes

- Victor Launcher is meant for BepInEx-based DLLs
- Error messages and mod status messages are found near the bottom of the menu next to Ship Status
- compatibility between large gameplay-overhaul mods still depends on the mods themselves
- this project is intended for mod management convenience, not for bypassing game restrictions or trust checks
- legacy versions of this mod (0.2.0 and older) keep support but do not have newer features available
- when installing the companion app or downloading the dll, you may see a windows popup saying "Windows protected your PC" or "Suspicious file blocked".
This is because it is an unrecognized app, though it is safe (feel free to run the file through virustotal or another antivirus)
