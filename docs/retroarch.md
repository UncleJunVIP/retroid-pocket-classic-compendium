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

## User Interface

| Setting         | Value |
|-----------------|-------|
| Menu Driver     | glui  |
| Display Overlay | Off   |

---

### Notification Visibility

| Notification Type                        | Enabled |
|------------------------------------------|---------|
| Input (Autoconfig) Failure Notifications | On      |
| Save State Notifications                 | On      |
| Screenshot Notifications                 | On      |
| All Other Notifications                  | Off     |

---

## Video

| Setting         | Value         |
|-----------------|---------------|
| Video Driver    | Vulkan        |
| Integer Scaling | On            |
| Aspect Ratio    | Core Provided |
| V-Sync          | On            |

---

## Audio

| Setting           | Value   |
|-------------------|---------|
| Resampler Quality | Highest |
| Menu Sounds       | All Off |

---

## Input

### RetroPad Binds - Port 1 Controls

| Control       | Button                     |
|---------------|----------------------------|
| Start Button  | Button 109 (Top Button)    |
| Select Button | Button 108 (Bottom Button) |

!!! note "My brain likes having `Start` assigned to the top button."

---

### Hotkeys

| Function                | Button                     |
|-------------------------|----------------------------|
| Hotkey Enable           | Select `[Button 108]`      |
| Menu Toggle             | Back Button `[Button 4]`   |
| Quit (Controller Combo) | Start + Select             |
| Fast-Forward (Toggle)   | R1 `[Button 103]`          |
| Rewind                  | L1 `[Button 102]`          |
| Audio Mute              | D-Pad Down `[Hat #0 Down]` |
| Load State              | L2 `[Button 104]`          |
| Save State              | R2 `[Button 105]`          |
| Show FPS (Toggle)       | X `[Button 99]`            |

!!! question "Why bind `Audio Mute`?"

    As mentioned earlier, I installed `Apple Music`. If I want to game and jam out to tunes this hotkey will mute *only* the emulation sound.

---

### Menu Controls

| Setting                         | Value             |
|---------------------------------|-------------------|
| Menu Swap OK and Cancel Buttons | Off (Japan style) |

---

## Saving

| Setting                                            | Value |
|----------------------------------------------------|-------|
| Sort Saves into Folders by Core Name               | Off   |
| Sort Save States into Folders by Core Name         | Off   |
| Sort Save into Folders by Content Directory        | On    |
| Sort Save States into Folders by Content Directory | On    |
| SaveRAM compression                                | On    |
| Auto Save State                                    | On    |
| Auto Load State                                    | On    |

---

## Configuration

| Setting                    | Value |
|----------------------------|-------|
| Save Configuration on Quit | On    |
| Save Remap Files on Quit   | On    |

---

## Directory

| Directory Type | Path                            |
|----------------|---------------------------------|
| System/BIOS    | `SD_CARD/Emulation/BIOS`        |
| Save Files     | `SD_CARD/Emulation/Saves`       |
| Save States    | `SD_CARD/Emulation/Save States` |
| Overlays       | `SD_CARD/Emulation/Overlays`    |

---

## Game Boy / Game Boy Color

### Core Options

| Setting             | Value                   |
|---------------------|-------------------------|
| GB Colorization     | Internal                |
| Internal Palette    | DMG                     |
| Interframe Blending | LCD Ghosting (Accurate) |

### Video Scaling

| Setting         | Value         |
|-----------------|---------------|
| Integer Scaling | Off           |
| Aspect Ratio    | Core provided |

### Shaders

| Setting       | Value                            |
|---------------|----------------------------------|
| Video Shaders | On                               |
| Shader Preset | Shaders Slang > Handheld > lcd3x |

---

## Game Boy Advance

### Core Options

| Setting             | Value |
|---------------------|-------|
| Color Correction    | On    |
| Interframe Blending | On    |

### Video Scaling

| Setting         | Value         |
|-----------------|---------------|
| Integer Scaling | On            |
| Aspect Ratio    | Core provided |

### Shaders

| Setting       | Value                            |
|---------------|----------------------------------|
| Video Shaders | On                               |
| Shader Preset | Shaders Slang > Handheld > lcd3x |

### On-Screen Overlay

| Setting                    | Value                                     |
|----------------------------|-------------------------------------------|
| Display Overlay            | On                                        |
| Autoload Preferred Overlay | On                                        |
| Overlay Preset             | gba-retroid-classic-integer-scale-rainbow |

---

## Nintendo Entertainment System

### Video Scaling

| Setting         | Value |
|-----------------|-------|
| Integer Scaling | Off   |
| Aspect Ratio    | Full  |

### Shaders

| Setting       | Value                                    |
|---------------|------------------------------------------|
| Video Shaders | On                                       |
| Shader Preset | Shaders Slang > CRT > newpixie-crt.slang |

---

## Super Nintendo Entertainment System

### Video Scaling

| Setting         | Value |
|-----------------|-------|
| Integer Scaling | Off   |
| Aspect Ratio    | Full  |

### Shaders

| Setting       | Value                                    |
|---------------|------------------------------------------|
| Video Shaders | On                                       |
| Shader Preset | Shaders Slang > CRT > newpixie-crt.slang |

---

## Sega Genesis

### Video Scaling

| Setting         | Value |
|-----------------|-------|
| Integer Scaling | Off   |
| Aspect Ratio    | Full  |

### Shaders

| Setting       | Value                                    |
|---------------|------------------------------------------|
| Video Shaders | On                                       |
| Shader Preset | Shaders Slang > CRT > newpixie-crt.slang |

---

## PlayStation

### Video Scaling

| Setting         | Value |
|-----------------|-------|
| Integer Scaling | Off   |
| Aspect Ratio    | Full  |

### Shaders

| Setting       | Value                                    |
|---------------|------------------------------------------|
| Video Shaders | On                                       |
| Shader Preset | Shaders Slang > CRT > newpixie-crt.slang |

