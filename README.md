# Emphase

### A minimal Windows 11 configuration using Mica transparency, acrylic blur, and WinUI 3 design language across the browser, terminal, taskbar, and File Explorer.

<p align="center">
  <img src="https://img.shields.io/badge/OS-Windows%2011-0078D4?style=for-the-badge&logo=windows11&logoColor=white" />
  <img src="https://img.shields.io/badge/Style-Minimal-1a1a2e?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/Browser-Firefox-FF7139?style=for-the-badge&logo=firefox&logoColor=white" />
  <img src="https://img.shields.io/badge/Effect-Mica-6e40c9?style=for-the-badge&logoColor=white" />
</p>

<p align="center"><b>Wallpaper:</b> <a href="https://wallhaven.cc/w/o5ly2l">wallhaven.cc/w/o5ly2l</a></p>

<picture><img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=0,2,2,5,30&height=4&section=header" width="100%"></picture>

## Preview

<p align="center">
  <img src="https://github.com/rakhalfps/emphase-rice/blob/a231e8b6273dc11c7851cfc27879980f56b853c9/MEDIA/1.gif" width="92%" />
</p>

<p align="center">
  <a href="https://github.com/rakhalfps/emphase-rice/blob/main/MEDIA/1.png">
    <img src="https://github.com/rakhalfps/emphase-rice/blob/main/MEDIA/1.png" width="46%" style="border:2px solid #30363d;border-radius:8px;margin:4px" />
  </a>
  <a href="https://github.com/rakhalfps/emphase-rice/blob/main/MEDIA/3.png">
    <img src="https://github.com/rakhalfps/emphase-rice/blob/main/MEDIA/3.png" width="46%" style="border:2px solid #30363d;border-radius:8px;margin:4px" />
  </a>
</p>

<picture><img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=6,11,20&height=4&section=header" width="100%"></picture>

## Tools

| Component | Tool |
|---|---|
| Firefox theme | [Firefox-WinUI](https://github.com/Lockframe/Firefox-WinUI) |
| Browser extension | [Zen Internet](https://addons.mozilla.org/en-US/firefox/addon/zen-internet/) |
| Taskbar / Start Menu | [Windhawk](https://windhawk.net/) |
| Global window blur | [DWMBlurGlass](https://github.com/Maplespe/DWMBlurGlass) |
| File Explorer blur | [ExplorerBlurMica](https://github.com/Maplespe/ExplorerBlurMica) |
| Cursor | [JimmyXD2 Cursor Pack](https://www.deviantart.com/jimmyxd2/art/1208233550) |

<picture><img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=12,19,28&height=4&section=header" width="100%"></picture>

## Setup

### Firefox

1. Open `about:support` and click **Open Folder** next to Profile Folder.
2. [Download Firefox-WinUI](https://github.com/Lockframe/Firefox-WinUI/archive/refs/heads/main.zip), extract it, and install the included `spinner-font.ttf`.
3. Copy the `chrome/` folder and `user.js` into your profile folder, then restart Firefox.
4. Open `about:config` and enable these keys:
   - `widget.windows.mica` — Mica on the browser frame
   - `widget.windows.mica.popups` — set to `1` (Acrylic) or `2` (Mica) for menus and panels
   - `browser.tabs.allow_transparent_browser` — extends Mica into the new tab page (optional)
5. Go to `about:support` and click **Clear startup cache** to apply all styles.
6. Install the [Zen Internet](https://addons.mozilla.org/en-US/firefox/addon/zen-internet/) extension.

Additional visual tweaks are available as boolean keys in `about:config`. Full list in the [Firefox-WinUI docs](https://github.com/Lockframe/Firefox-WinUI#settings).

<picture><img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=24,30,6&height=4&section=header" width="100%"></picture>

### Windhawk

1. Install [Windhawk](https://windhawk.net/) and open it.
2. From the **Explore** tab, install **Windows 11 Taskbar Styler** and **Windows 11 Start Menu Styler**.
3. Open each mod's **Settings** tab, paste the config below, and save. Changes apply immediately.
   - Taskbar: [pastebin.com/qM0WLtch](https://pastebin.com/qM0WLtch)
   - Start Menu: [pastebin.com/834WW7me](https://pastebin.com/834WW7me)

<picture><img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=3,9,17&height=4&section=header" width="100%"></picture>

### DWMBlurGlass

Hooks into the Desktop Window Manager to apply Mica or Acrylic effects to all title bars globally.

1. Download from the [releases page](https://github.com/Maplespe/DWMBlurGlass/releases) and extract to a permanent location.
2. Run `DWMBlurGlass.exe` and click **Install**. If nothing happens, go to the **Symbols** tab, click **Download**, then try Install again.
3. Set effect to **Mica** and blur method to **CustomBlur**. Save to apply live.

> Only download from the official GitHub releases page. Impersonation campaigns distributing malware-bundled versions exist.

> Do not run alongside MicaForEveryone as both target the same DWM pipeline.

<picture><img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=15,22,4&height=4&section=header" width="100%"></picture>

### ExplorerBlurMica

Applies Mica or Acrylic to File Explorer without modifying system files.

1. Download from the [releases page](https://github.com/Maplespe/ExplorerBlurMica/releases) and extract to a permanent location.
2. Right-click `register.cmd` and run as administrator. Explorer restarts automatically.
3. Edit `config.ini` to set your preferred effect (`2` = Mica, `1` = Acrylic, `0` = Blur) and reopen Explorer.

To uninstall, run `uninstall.cmd` as administrator.

<picture><img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=27,5,13&height=4&section=header" width="100%"></picture>

### Windows Terminal

Open **Settings > Appearance** for your active profile. Enable **Use acrylic material** and set **Background opacity** to `30`.

<picture><img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=8,18,25&height=4&section=header" width="100%"></picture>

### Cursor

1. Download and extract the [cursor pack](https://www.deviantart.com/jimmyxd2/art/1208233550).
2. Run `main.cpl` to open Mouse Properties, go to the **Pointers** tab, and apply the scheme. If a `.inf` file is included, right-click it and select **Install** instead.
