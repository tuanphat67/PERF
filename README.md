# PERF 0.3.7

<p align="center">
  <img src="docs/images/hero.jpg" alt="PERF with its five themes: PERF Classic, Cosmos, Astronaut, Shinobi and Night Racer" width="100%">
</p>

<p align="center">
  <b>A clean, lightweight hardware monitor for Windows.</b><br>
  CPU, GPU, RAM, storage, fans, battery and network in one window, with five illustrated themes,<br>
  an always-on-top mini overlay, a 30-second temperature check and a self-reverting CPU cool-down.
</p>

<p align="center">
  <a href="https://github.com/tuanphat67/PERF/releases/latest"><img src="https://img.shields.io/github/v/release/tuanphat67/PERF?label=Download&style=for-the-badge&color=22c3e6" alt="Download the latest release"></a>
  <img src="https://img.shields.io/badge/Windows-10%20%7C%2011%20x64-0b0f14?style=for-the-badge&logo=windows" alt="Windows 10 and 11, x64">
  <img src="https://img.shields.io/badge/Language-English%20%7C%20Ti%E1%BA%BFng%20Vi%E1%BB%87t-0b0f14?style=for-the-badge" alt="English and Vietnamese">
  <img src="https://img.shields.io/badge/Price-Free-8a5cf6?style=for-the-badge" alt="Free">
</p>

<p align="center">
  <a href="https://github.com/tuanphat67/PERF/releases/latest"><b>⬇ Download PERF for Windows</b></a>
  &nbsp;·&nbsp; <a href="#install-in-one-minute">Install</a>
  &nbsp;·&nbsp; <a href="#five-themes">Themes</a>
  &nbsp;·&nbsp; <a href="#faq">FAQ</a>
</p>

> **English and Vietnamese:** PERF picks English or Vietnamese from your Windows display language on first launch. Switch any time under **Settings → Appearance → Language**.

---

## Highlights

| | |
|---|---|
| 📊 **Everything at a glance** | CPU, GPU, RAM, storage, fans and pumps, battery and network on one dashboard, with a 1-minute, 10-minute or 1-hour chart and per-moment values on hover. |
| ⏺️ **Record to CSV** | Click **Record** while you game or render, then open the CSV in Excel to compare sessions. |
| 🌡️ **Temperature in the tray** | The tray icon shows your CPU temperature live, turning green, amber or red as it nears your warning threshold. |
| 🔔 **Heat alerts** | Get a Windows notification when the CPU or GPU stays above your threshold. Click it to jump to **Thermals**. |
| 🪟 **Always-on-top mini overlay** | Sits in a screen corner and is click-through, so it never gets in the way of games or work. Show or hide it from anywhere with **Ctrl + Shift + O**. |
| 🔍 **What's using my PC?** | Click the CPU or RAM tile to see the five apps using the most, grouped by name. |
| 🎨 **Five illustrated themes** | PERF Classic, Cosmos, Astronaut, Shinobi and Night Racer, each with its own artwork, icon and colour palette. |
| 🌐 **English and Vietnamese** | Switch the whole interface, overlay and tray menu instantly, no restart needed. |
| 🔄 **One-click updates** | The version tag in the corner tells you when a new release is out and what's new in it. Click **Update now** and PERF downloads, verifies and installs it, then reopens. |
| 🌡️ **Measure and cool down** | Record temperatures for 30 seconds under your real workload. Cap the CPU at 60, 75 or 90% for 10 minutes, then it restores itself. |
| 🔒 **Honest and safe** | No made-up numbers: sensors that report nothing show *Not available*. PERF collects no personal data and never drives your fans. |
| 🪶 **Lightweight** | Under 1% CPU while running in the background on our test laptop. Minimises to the system tray. |

## Five themes

Switch under **Settings → Appearance**, preview instantly, then click **Save settings**. The language selector lives in the same panel.

<p align="center">
  <img src="docs/images/theme-picker.png" alt="Theme picker in Settings" width="820">
</p>

<table>
  <tr>
    <td width="50%"><img src="docs/images/theme-cosmos.jpg" alt="Cosmos theme"><br><b>🪐 Cosmos</b>: a ringed gas giant, violet nebula and a deep star field.</td>
    <td width="50%"><img src="docs/images/theme-astronaut.jpg" alt="Astronaut theme"><br><b>👨‍🚀 Astronaut</b>: Earth's night-side horizon seen from a space station.</td>
  </tr>
  <tr>
    <td><img src="docs/images/theme-shinobi.jpg" alt="Shinobi theme"><br><b>🥷 Shinobi</b>: a full moon over a misty pagoda and bamboo.</td>
    <td><img src="docs/images/theme-night-racer.jpg" alt="Night Racer theme"><br><b>🏎️ Night Racer</b>: a rain-soaked night circuit streaked with tail lights.</td>
  </tr>
  <tr>
    <td><img src="docs/images/theme-classic.jpg" alt="PERF Classic theme"><br><b>📈 PERF Classic</b>: glowing circuit traces and a cyan oscilloscope wave.</td>
    <td align="center"><img src="docs/images/theme-icons.png" alt="The five theme icons" width="90%"><br>Every theme ships with its own 3D icon.</td>
  </tr>
</table>

> The theme screenshots use simulated data so every tile is filled. On a real machine, readings depend on the sensors your hardware exposes.

## Chart history and session recording

- **Chart range:** above the chart on the Overview page, pick **1 min**, **10 min** or **1 hour**. PERF keeps the last hour of every sensor in memory from the moment it opens, even while it sits in the tray.
- **Record:** click **● Record** to start writing every sensor to a CSV file once per sample. The button turns into **■ Stop** with the elapsed time; recording keeps going while PERF is in the tray. Click **Stop** when you're done.
- **Where the file goes:** `Documents\PERF\PERF-<date>-<time>.csv`. Click **Open folder** under the chart to find it.
- **File format:** one row per sample with `Time`, `Elapsed (s)` and one column per sensor, named *Device | Sensor (unit)*. Numbers use a dot as the decimal separator. An empty cell means the sensor had no reading at that moment, which is different from a real 0. Sensors that appear after you start recording are not added.

> Tip: record a few minutes of the same game before and after cleaning your fans or repasting the CPU, then compare the `CPU Package (°C)` columns.

## Top apps

Click the **CPU** or **RAM** tile on the Overview page. Below the 60-second chart, **Top apps by CPU** or **Top apps by RAM** lists the five apps using the most right now. Processes with the same name are added together (a browser with 20 helper processes shows as one row, marked *×20*). PERF only measures processes while this card is on screen.

> Apps running as administrator may be missing while PERF itself runs without admin rights. Enable advanced mode to see them.

## Tray temperature and heat alerts

- **Live tray icon:** the PERF icon in the system tray becomes a small tile with the current temperature. It follows **Settings → Sampling & alerts → Pinned metric** when that metric is a temperature, otherwise the CPU. Hover it for the exact reading.

  | Colour | Meaning |
  |---|---|
  | 🟢 Green | Below *threshold − 5 °C* |
  | 🟡 Amber | Within 5 °C of the threshold |
  | 🔴 Red | At or above the threshold |

- **Heat alerts:** set a **Warning threshold** (40–110 °C) and **Time above threshold** (5–60 s). When the CPU or GPU stays that hot for that long, Windows shows a notification. Click it to open **Thermals**. You get one alert per hot spell; it re-arms after the temperature drops back.
- Both are on by default. Turn them off with **Show temperature on the tray icon** and **Notify me when the CPU / GPU stays above the threshold**, then click **Save settings**.

> Can't see the icon? Windows may hide new tray icons. Open **Windows Settings → Personalization → Taskbar → Other system tray icons** and turn **PERF** on.

## Mini overlay

A small always-on-top window in the corner of your screen. By default it shows CPU, GPU and RAM usage plus temperatures when available. Choose **Compact rows**, **Horizontal strip** or **Usage bars** and adjust position, size, background opacity and one to three metrics under **Settings → Mini overlay**. **Use theme overlay preset** fills in a layout that matches the current theme.

**Hotkey:** press **Ctrl + Shift + O** anywhere, even in a game, to show or hide the overlay. Pick another combination (or **Off**) under **Settings → Mini overlay → Show/hide hotkey**. If the overlay's position is set to **Off**, the hotkey shows it in the top-right corner until you press it again. Clicking **Save settings** returns the overlay to the position you chose. If another app already uses the combination, PERF tells you when you save; pick a different one.

<p align="center">
  <img src="docs/images/overlays.png" alt="The three overlay layouts in all five themes" width="100%">
</p>

## Temperature check and CPU cool-down

<img src="docs/images/cooling.png" alt="Temporary CPU cool-down panel" width="360" align="right">

- **Temperature check:** start a measurement while a game or heavy task is running. PERF records the starting, current and peak temperature over 30 seconds. It never generates load on its own.
- **Temporary CPU cool-down:** cap the maximum processor state at **60%, 75% or 90%** for 10 minutes, on both AC and battery power.
- **Always reverted:** PERF edits a copy of your power plan and restores the original when time runs out or when you quit, even after a crash or power loss. **Restore previous power plan** undoes it immediately.
- **Fans and pumps:** the **Fans and pumps** card shows every RPM and PWM channel your machine reports. Fans stay under firmware or vendor-software control. On Lenovo laptops, PERF also reads fan speed through Lenovo WMI.

<br clear="right">

## Install in one minute

1. Download `PERF-<version>-x64.msi` from [**Releases**](https://github.com/tuanphat67/PERF/releases/latest).
2. Run the installer. The .NET runtime is bundled, so nothing else is needed.
3. Launch **PERF** from the Start menu. The main window and the mini overlay appear right away.

**Advanced sensors (recommended):** the installer includes the signed **PawnIO** driver, which unlocks extra CPU temperature and power readings. Accept the UAC prompt when asked. If you skipped it, open **Settings → Sensor sources**, click **Install bundled PawnIO**, then quit and reopen PERF.

**Update:** the version tag at the bottom of the sidebar shows **Latest** or **Update to x.y.z**. When PERF finds a new version in the background it also shows a notification; click it to open the update dialog. The dialog lists **What's new** in your language. Click **Update now**: PERF downloads the new installer from GitHub, checks its SHA-256, closes cleanly, installs and reopens. You can also quit PERF and run a newer installer by hand. Your settings are kept either way.

**Uninstall:** quit PERF, then remove it from **Settings → Apps → Installed apps** in Windows.

### Requirements

- Windows 10 or 11, 64-bit (x64).
- Laptop or desktop. Available readings depend on your hardware and drivers.

## Tips

- Click **X** to send PERF to the system tray; the overlay and the tray temperature keep updating. Double-click the tray icon to bring it back.
- Pin a GPU or SSD temperature under **Settings → Sampling & alerts → Pinned metric** to show it on the tray icon instead of the CPU.
- Click the **Fans and pumps** card to see every RPM and PWM channel; **Reset min/max** starts the session statistics over.
- On the chart, pick a metric below it and hover to read any moment. Switch to **1 hour** to see a whole gaming session.
- **Settings → Restore defaults** resets every option and returns your power plan to how it was.

## FAQ

<details>
<summary><b>Why does GPU temperature show "– °C"?</b></summary>

Usually because the machine only has integrated graphics (for example Intel UHD Graphics). The iGPU shares the CPU die and has no temperature sensor of its own, so PERF leaves it blank instead of guessing. Discrete NVIDIA and AMD GPUs report their temperature normally.
</details>

<details>
<summary><b>Why do some tiles say "Not available"?</b></summary>

Your drivers or firmware don't expose that reading. Installing **PawnIO** and allowing advanced mode unlocks more CPU temperature and power sensors. Some GPU, SSD and fan readings still depend on the device.
</details>

<details>
<summary><b>How do I report a problem?</b></summary>

Open **Settings → Sensor sources** and click **Copy diagnostic report**. It copies the PERF and Windows versions, sensor sources and current readings, with no machine name, user name or file paths. Paste it into a new issue on [GitHub Issues](https://github.com/tuanphat67/PERF/issues) together with what you expected and what happened.
</details>

<details>
<summary><b>Does PERF control fans or overclock?</b></summary>

No. PERF only reads sensors. The cool-down feature temporarily lowers the maximum processor state through the Windows power plan and always reverts it.
</details>

<details>
<summary><b>Does PERF collect my data or phone home?</b></summary>

No. The only network request PERF makes is a version check against this repository's public GitHub Releases (about 45 seconds after launch, then every 12 hours) and the installer download when you choose to update. No hardware data or personal information is sent. Turn off **Check for updates automatically** in Settings to stop the background check. Settings are stored locally in `%LocalAppData%\PERF`.
</details>

<details>
<summary><b>Windows SmartScreen warns about the installer</b></summary>

The PERF installer is not code-signed yet, so Windows may show a warning. Only download PERF from the official Releases page. If you trust the file, choose **More info → Run anyway**.
</details>

<details>
<summary><b>A cool-down session seems stuck after a sudden shutdown</b></summary>

Open PERF or sign in to Windows again and the recovery runs automatically. If it still isn't restored, open `%LocalAppData%\PERF\cooling.json`, copy the value of `Original`, and run `powercfg /setactive <value>` in PowerShell, or pick your previous plan in Power Options.
</details>

## License

PERF is **free software with all rights reserved** by its author. You may download the official installer from Releases and use it free of charge. Copying, modifying, redistributing or selling PERF, its code, artwork or icons is not permitted without the author's written permission. See [LICENSE](LICENSE).

PERF bundles third-party components that keep their own licenses: LibreHardwareMonitorLib (MPL-2.0), HidSharp, the .NET runtime and the PawnIO installer. See [THIRD-PARTY.txt](THIRD-PARTY.txt).
