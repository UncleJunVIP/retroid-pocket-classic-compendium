# Retroid Pocket Classic Compendium 📓

It is no secret that I am *addicted* to retro gaming handhelds.

I wanted a place to capture things about my Retroid Pocket Classic setup.

I don't claim to be an expert and will likely have done something stupid or wrong.

For more detail from an actual expert, go check out [Retro Game Corps'](https://retrogamecorps.com) guides and videos.

If it exists, Russ has a video for it.

*With that in mind, here goes nothing!*

❤️

---

## Wrangling the Apps 🐂➰🤠

After the initial Retroid-provided setup, I installed the following:

1. [Emulation Station Desktop Edition](https://es-de.org) (ES-DE), paid, but extremely reasonable (~$5)
2. [Obtainium](https://github.com/ImranR98/Obtainium)
3. [RetroArch (AArch64) Nightly Config](https://apps.obtainium.imranr.dev) via Obtainium App Configuration
    - use the filter function to find the RetroArch configuration
4. [F-Droid](https://f-droid.org/en/)
5. [Aurora Store](https://f-droid.org/en/packages/com.aurora.store/) via F-Droid
6. [Primitive FTPd](https://f-droid.org/en/packages/org.primftpd/) via F-Droid
7. [LocalSend](https://f-droid.org/en/packages/org.localsend.localsend_app/) via F-Droid
8. [Tailscale](https://f-droid.org/en/packages/com.tailscale.ipn/) via F-Droid

---

## RetroArch Configuration ⚙️

### Installed Emulator Cores

- Game Boy / Color (Gambatte)
- Game Boy Advance (gpSP / mGBA)
- Nintendo Entertainment System (Nestopia)
- Super Nintendo Entertainment System (Snes9x)
- Sega Genesis (Genesis Plus GX)
- PlayStation (SwanStation)

These are all recommended by
RGC's [RetroArch Starter Guide](https://retrogamecorps.com/2022/02/28/retroarch-starter-guide/)

Why only these systems? This is what I play. I'm a simple man.

---

### Global RetroArch Settings

These settings will be displayed as nested lists. The nesting follows the navigational hierarchy.

Settings will be displayed as Setting Name: Value

Notes included when for sections when spelling out the value of every setting is cumbersome.

If a setting is not listed, a safe assumption is I am using the default.

#### User Interface

- Menu Driver: glui
- On-Screen Notifications
    - Notification Visibility (Everything Off Except For)
        - Input (Autoconfig) Failure Notifications
        - Save State Notifications
        - Screenshot Notifications
- On-Screen Overlay
    - Display Overlay: Off

---

#### Video

- Output
    - Video Driver: Vulkan
- Scaling
    - Integer Scaling: On
    - Aspect Ratio: Core Provided
- Synchronization
    - V-Sync: On

---

#### Audio

- Output
    - Resampler Quality: Highest
- Menu Sounds (All Off)

---

#### Input

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

#### Saving

- Sort Saves into Folders by Core Name: Off
- Sort Save States into Folders by Core Name: Off
- Sort Save into Folders by Content Directory: On
- Sort Save States into Folders by Content Directory: On
- SaveRAM compression: On
- Auto Save State: On
- Auto Load State: On

```
Saving Notes

These first four options make it so RetroArch behaves like my beloved NextUI.

Auto Save / Load allows you to quit with Start + Select and not worry! 
A save state will be made on quit and loaded on start. Seamless!
```

---

#### Configuration

- Save Configuration on Quit: On
- Save Remap Files on Quit: On

---

#### Directory

- System/BIOS: `SD_CARD/Emulation/BIOS`
- Save Files: `SD_CARD/Emulation/Saves`
- Save States: `SD_CARD/Emulation/Save States`
- Overlays: `SD_CARD/Emulation/Overlays`

```
Directory Notes

This again is to NextUI-ify this Android setup. 
I also have ES-DE pointed at SD_CARD/Emulation/ROMs for games.

Why are all these directories under Emulation? Good question!

Android is silly with file permissions for non-rooted devices. 
This scheme allows you to expose your content via Primitive FTPd.
```

---

### Emulator Specific Settings

For these configurations, make use of the `Save Content Directory Overrides` to apply to all games for a system.

#### Game Boy / Game Boy Color (Gambatte)

##### Core Options

- GB Colorization: Internal
- Internal Palette: DMG
- Interframe Blending: LCD Ghosting (Accurate)

##### Video -> Scaling

- Integer Scaling: Off
- Aspect Ratio: Core provided

##### Shaders

- Video Shaders: On
- Load Preset
    - Shaders Slang
        - Handheld
            - lcd3x

---

#### Game Boy Advance (gpSP / mGBA)

##### Core Options

- Color Correction: On
- Interframe Blending: On

##### Video -> Scaling

- Integer Scaling: On
- Aspect Ratio: Core provided

##### Shaders

- Video Shaders: On
- Load Preset
    - Shaders Slang
        - Handheld
            - lcd3x

##### On-Screen Overlay

- Display Overlay: On
- Autoload Preferred Overlay: On
- Overlay
  Preset: [gba-retroid-classic-integer-scale-rainbow](https://github.com/timbueno/retroid-pocket-classic-overlays/blob/main/retroid-classic-gba-overlays/gba-retroid-classic-integer-scale-rainbow.png)
    - Thanks, [@timbueno](https://github.com/timbueno)!

```
Bueno's overlays are vendored here for completeness.
```

---

#### Nintendo Entertainment System (Nestopia)

##### Video -> Scaling

- Integer Scaling: Off
- Aspect Ratio: Full (The RPC's aspect ratio is close enough)

##### Shaders

- Video Shaders: On
- Load Preset
    - Shaders Slang
        - CRT
            - newpixie-crt.slang

---

#### PlayStation (SwanStation)

##### Video -> Scaling

- Integer Scaling: Off
- Aspect Ratio: Full (The RPC's aspect ratio is close enough)

##### Shaders

- Video Shaders: On
- Load Preset
    - Shaders Slang
        - CRT
            - newpixie-crt.slang

---

## ES-DE Configuration

### System Name Customization

✨ *To perform any of these changes, you will need a copy of
[es_systems.xml](https://gitlab.com/es-de/emulationstation-de/-/blob/master/resources/systems/android/es_systems.xml)* ✨

#### Renaming Systems

To rename a system, simply change the value of the `<fullname>` tag for the corresponding `<system>`.

---

#### Change System Display Order

Use the following snippet as an example to edit your `es_systems.xml` file.

(Note the `<command>` tags have been omitted for clarity.)

```xml

<systemList>
    <system>
        <name>gb</name>
        <fullname>Game Boy</fullname>
        <systemsortname>001 - BTK</systemsortname>
        <path>%ROMPATH%/gb</path>
        <extension>.bs .BS .cgb .CGB .dmg .DMG .gb .GB .gbc .GBC .sgb .SGB .sfc .SFC .smc .SMC .7z .7Z .zip .ZIP
        </extension>
        ...
        <platform>gb</platform>
        <theme>gb</theme>
    </system>
    <system>
        <name>gbc</name>
        <fullname>Game Boy Color</fullname>
        <systemsortname>002 - BTK</systemsortname>
        <path>%ROMPATH%/gbc</path>
        <extension>.bs .BS .cgb .CGB .dmg .DMG .gb .GB .gbc .GBC .sgb .SGB .sfc .SFC .smc .SMC .7z .7Z .zip .ZIP
        </extension>
        ...
        <platform>gbc</platform>
        <theme>gbc</theme>
    </system>
</systemList>
```

ES-DE uses the `<systemsortname>` tag to determine system order.

I went with this naming scheme of `Platform Order - My Initials`. Use whatever makes sense to you.

To make sure ES-DE uses your custom ordering, be sure to set `Systems Sorting` to `Full Names or Custom` under
`UI Settings`.

