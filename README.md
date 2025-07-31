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

1. [Emulation Station Desktop Edition](https://es-de.org) (paid, but extremely reasonable)
2. [Obtainium](https://github.com/ImranR98/Obtainium)
3. [RetroArch (AArch64) Nightly Config](https://apps.obtainium.imranr.dev) (use the filter function)
4. [F-Droid](https://f-droid.org/en/)
5. [Primitive FTPd](https://f-droid.org/en/packages/org.primftpd/) via F-Droid
6. [Tailscale](https://f-droid.org/en/packages/com.tailscale.ipn/) via F-Droid
7. [Aurora Store](https://f-droid.org/en/packages/com.aurora.store/) via F-Droid

---

## High-Level RetroArch Configuration ⚙️

### Emulator Cores

- Game Boy / Color (Gambatte)
- Game Boy Advance (mGBA)
- Nintendo Entertainment System (Nestopia)
- Super Nintendo Entertainment System (Snes9x)
- Sega Genesis (Genesis Plus GX)
- PlayStation (SwanStation)

These are all recommended by
RGC's [RetroArch Starter Guide](https://retrogamecorps.com/2022/02/28/retroarch-starter-guide/)

Why only these systems? This is what I play. I'm a simple man.

### Global RetroArch Settings

These settings will be displayed as nested lists. The nesting follows the navigational hierarchy.

Settings will be displayed as Setting Name: Value

Notes included when for sections when spelling out the value of every setting is cumbersome.

If a setting is not listed, a safe assumption is I am using the default.

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
    - Hotkey Enable: Select [Button 108] (Button Button that defaults as Start)
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

```
Saving Notes

These first four options make it so RetroArch behaves like my beloved NextUI (MinUI).

Auto Save / Load allows you to quit with Start + Select and not worry! 
A save state will be made on quit and loaded on start. Seamless!
```

---

### Configuration

- Save Configuration on Quit: On
- Save Remap Files on Quit: On

---

### Directory

- System/BIOS: `SD_CARD/BIOS`
- Save Files: `SD_CARD/Saves`
- Save States: `SD_CARD/Save States`

```
Directory Notes

This again is to NextUI-ify this Android setup. 
I also have ES-DE pointed at SD_CARD/ROMs for games.
```

---