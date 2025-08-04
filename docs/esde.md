## UI Settings

| Setting                | Value      |
|------------------------|------------|
| Theme                  | MinUI Menu |
| Menu Opening Animation | None       |
| Launch Screen Duration | Disable    |
| Display Clock          | On         |

## Sound Settings

| Setting                                         | Value |
|-------------------------------------------------|-------|
| Play Audio for Game List and System View Videos | Off   |
| Play Audio for Media Viewer Videos              | Off   |
| Play Audio for Screensaver Videos               | Off   |
| Enable Navigation Sounds                        | Off   |

## Input Device Settings

| Setting                      | Value |
|------------------------------|-------|
| Enable Touch Overlay         | Off   |
| Swap the A/B and X/Y Buttons | Off   |

## Other Settings / Alternative Emulators

!!! info "Assign each system to the corresponding core you installed earlier"

---

## Utilities / Game Importer

!!! info "This tool's name is a misnomer!"

This tool has been recently added to ES-DE and allows you to add Android Apps and Android Games to the ES-DE menu.

1. Select `Game Importer`
2. For the `Import to System` option select the type of thing you want to import (e.g. Android Apps / Android Games)
3. Scroll down to `Start`
4. When the list of apps appears, check each app that you want to add to the selected `Import to System` option.
5. ES-DE will "rescan" your ROMs and the selected apps will appear in their corresponding section.

---

## System Name Customization

!!! info "Go grab a copy of es_systems.xml"

    To perform any of these changes, you will need a copy of [es_systems.xml](https://gitlab.com/es-de/emulationstation-de/-/blob/master/resources/systems/android/es_systems.xml).

### Renaming Systems

To rename a system, simply change the value of the `<fullname>` tag for the corresponding `<system>`.

---

### Change System Display Order

Use the following snippet as an example to edit your `es_systems.xml` file.

!!! info "Note the `<command>` tags have been omitted for clarity."

``` xml
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

