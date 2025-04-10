# Addon Preferences

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/H_rOdtkc1Yo?si=Ulj7oOo2bJ6C9rjq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</p>

The addon preferences contain all of the global PBR Painter preferences and settings that are applied across your projects/files. 

## General

### Check for Updates

This button does a quick check to see if you're using the latest version of PBR Painter. Note that it requires an internet connection. If a later version is found, you'll be provided with links to your marketplace of choice (Superhive (formely Blender Market), Flipped Normals or Gumroad).

### Assets Directory

If you are using Blender 3+, it is recommended that you choose an asset directory, within the addon preferences. This will create a new filepath to tell Blender where your PBR Painter assets will be stored. Note that a more detailed guide to using the asset browser with PBR Painter is provided [here.](./asset_browser.md)

### General preferences

There are three other general PBR Painter settings:

- **Show UI in sidebar:** This option shows the *entire* PBR Painter UI within the sidebar/N-panel in any Blender workspace. This is switched off by default, as the intended use of PBR Painter is within the dedicated workspace, but is available should you need to access the addon from other workspaces.

- **Hide PBR Painter UI in other workspaces:** This option, on by default, hides the PBR Painter UI from the Properties -> Tools panel within all workspaces other than the dedicated PBR Painter workspace. Note this is independent from the Show UI in sidebar option.

- **Auto-refreh materials:** This dropdown controls how materials are auto-refreshed after any updates. This is intended to reduce constant updating which can be computationally heavy, especially when using Eevee. There are three possible options:
    - *Cycles only (default):* Only auto-refreshes in Cycles, reducing computational load in Eevee.
    - *Never:* Never auto-refresh, meaning that you will need to actively refresh the material after any updates, regardless of render engine. Note that this can be switched on/off for each specific material.
    - *Always:* Always refreshes materials after every change. This can be computationally demanding but removes the requirement for the user to manually refresh.

### Image saving preferences

These preferences control how images within PBR Painter are saved, allowing for more optimised workflows that do not need to be setup for each individual project file.

- *Autosave images:* Controls whether images within PBR Painter materials are saved automatically. If on, you will also be opted to specify a *Time between saves* in minutes, controlling the autosave frequency.
- *Use relative paths:* Controls whether to use relative (versus absolute) paths for images within PBR Painter materials.
- *Save Method:* Controls how images are saved, either **Pack** or **Save Externally**. If saving externally by default you will be given additional preferences:
    - *Directory type:* Controls whether to use a subdirectory of the current blend file, or an absolute directory. If subdirectory is used, you will also be asked to specify the subdirectory name (*PBRPainterImages* by default).
    - *Format, Color, Color Depth & Compression:* Format and color settings to use for saved images.

### Texture tags

Texture tags are strings that are used to identify images associated with different channels in your material when importing multiple textures (multi-import). You can specify unlimited tags for each channel, separated with semicolons (;).