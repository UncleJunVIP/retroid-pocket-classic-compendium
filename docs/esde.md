## System Name Customization

✨ *To perform any of these changes, you will need a copy of
[es_systems.xml](https://gitlab.com/es-de/emulationstation-de/-/blob/master/resources/systems/android/es_systems.xml)* ✨

### Renaming Systems

To rename a system, simply change the value of the `<fullname>` tag for the corresponding `<system>`.

---

### Change System Display Order

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

