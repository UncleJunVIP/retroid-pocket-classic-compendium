## Update all the things!

From the RetroArch main menu, navigate to `Online Updater`.

Find each of the following and select them to make sure everything is up to date.

- Update Core Info Files
- Update Assets
- Update Controller Profiles
- Update Cheats
- Update Databases
- Update Shaders

---

## Emulator Cores

From the RetroArch main menu, navigate to `Online Updater -> Core Downloader`.

These are the cores that I installed.

| Console                             | Emulator Core   |
|-------------------------------------|-----------------|
| Game Boy / Color                    | Gambatte        |
| Game Boy Advance                    | gpSP / mGBA     |
| Nintendo Entertainment System       | Nestopia        |
| Super Nintendo Entertainment System | Snes9x          |
| Sega Genesis                        | Genesis Plus GX |
| PlayStation                         | SwanStation     |

These are all recommended by
RGC's [RetroArch Starter Guide](https://retrogamecorps.com/2022/02/28/retroarch-starter-guide/).

Why only these systems? This is what I play. I'm a simple man.

---

## Global RetroArch Settings

These settings will be displayed as nested lists. The nesting follows the navigational hierarchy.

Settings will be displayed as Setting Name: Value

Notes included when for sections when spelling out the value of every setting is cumbersome.

If a setting is not listed, a safe assumption is I am using the default.

---

### User Interface

- Menu Driver: glui
- On-Screen Notifications
    - Notification Visibility (Everything Off Except For)
        - Input (Autoconfig) Failure Notifications
        - Save State Notifications
        - Screenshot Notifications
- On-Screen Overlay
    - Display Overlay: Off

---

### Video

- Output
    - Video Driver: Vulkan
- Scaling
    - Integer Scaling: On
    - Aspect Ratio: Core Provided
- Synchronization
    - V-Sync: On

---

### Audio

- Output
    - Resampler Quality: Highest
- Menu Sounds (All Off)

---

### Input

- RetroPad Binds
    - Port 1 Controls
        - Start Button: Button 109 (Top Button, defaults as Select)
            - I like the Start Button on top. Sue me.
        - Select Button: Button 108 (Bottom Button, defaults as Start)
- Hotkeys
    - Hotkey Enable: Select [Button 108] (Bottom Button that defaults as Start)
    - Menu Toggle: Back Button [Button 4]
    - Quit (Controller Combo): Start + Select
    - Fast-Forward (Toggle): R1 [Button 103]
    - Rewind: L1 [Button 102]
    - Load State: L2 [Button 104]
    - Save State: R2 [Button 105]
    - Show FPS (Toggle): X [Button 99]
- Menu Controls
    - Menu Swap OK and Cancel Buttons: Off (Japan style. A = Select / Confirm, B = Back)

---

### Saving

- Sort Saves into Folders by Core Name: Off
- Sort Save States into Folders by Core Name: Off
- Sort Save into Folders by Content Directory: On
- Sort Save States into Folders by Content Directory: On
- SaveRAM compression: On
- Auto Save State: On
- Auto Load State: On

!!! info "Saving Notes"

    These first four options make it so RetroArch behaves like my beloved NextUI.

    Auto Save / Load allows you to quit with Start + Select and not worry!
    A save state will be made on quit and loaded on start. Seamless!

---

### Configuration

- Save Configuration on Quit: On
- Save Remap Files on Quit: On

---

#### Directory

- System/BIOS: `SD_CARD/Emulation/BIOS`
- Save Files: `SD_CARD/Emulation/Saves`
- Save States: `SD_CARD/Emulation/Save States`
- Overlays: `SD_CARD/Emulation/Overlays`

!!! info "Directory Notes"

    This again is to NextUI-ify this Android setup.
    I also have ES-DE pointed at `SD_CARD/Emulation/ROMs` for games.

    Why are all these directories under `Emulation`? Good question!
    
    Android is silly with file permissions for non-rooted devices.
    This scheme allows you to expose your content via Primitive FTPd.

---

### Game Boy / Game Boy Color

#### Core Options

- GB Colorization: Internal
- Internal Palette: DMG
- Interframe Blending: LCD Ghosting (Accurate)

#### Video -> Scaling

- Integer Scaling: Off
- Aspect Ratio: Core provided

#### Shaders

- Video Shaders: On
- Load Preset
    - Shaders Slang
        - Handheld
            - lcd3x

---

### Game Boy Advance

#### Core Options

- Color Correction: On
- Interframe Blending: On

#### Video -> Scaling

- Integer Scaling: On
- Aspect Ratio: Core provided

#### Shaders

- Video Shaders: On
- Load Preset
    - Shaders Slang
        - Handheld
            - lcd3x

#### On-Screen Overlay

- Display Overlay: On
- Autoload Preferred Overlay: On
- Overlay
  Preset: [gba-retroid-classic-integer-scale-rainbow](https://github.com/timbueno/retroid-pocket-classic-overlays/blob/main/retroid-classic-gba-overlays/gba-retroid-classic-integer-scale-rainbow.png)
    - Thanks, [@timbueno](https://github.com/timbueno)!

```
Bueno's overlays are vendored here for completeness.
```

---

### Nintendo Entertainment System

#### Video -> Scaling

- Integer Scaling: Off
- Aspect Ratio: Full (The RPC's aspect ratio is close enough)

#### Shaders

- Video Shaders: On
- Load Preset
    - Shaders Slang
        - CRT
            - newpixie-crt.slang

---

### Super Nintendo Entertainment System

#### Video -> Scaling

- Integer Scaling: Off
- Aspect Ratio: Full (The RPC's aspect ratio is close enough)

#### Shaders

- Video Shaders: On
- Load Preset
    - Shaders Slang
        - CRT
            - newpixie-crt.slang

---

### Sega Genesis

#### Video -> Scaling

- Integer Scaling: Off
- Aspect Ratio: Full (The RPC's aspect ratio is close enough)

#### Shaders

- Video Shaders: On
- Load Preset
    - Shaders Slang
        - CRT
            - newpixie-crt.slang

---

### PlayStation

#### Video -> Scaling

- Integer Scaling: Off
- Aspect Ratio: Full (The RPC's aspect ratio is close enough)

#### Shaders

- Video Shaders: On
- Load Preset
    - Shaders Slang
        - CRT
            - newpixie-crt.slang

---