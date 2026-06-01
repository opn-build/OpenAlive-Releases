<div align="center">
  <h1>OpenAlive</h1>
  <p>Keep your Windows session active. Lightweight, private, multilingual.</p>

  [![Version](https://img.shields.io/github/v/release/opn-build/OpenAlive-Releases?label=version&color=4caf50)](https://github.com/opn-build/OpenAlive-Releases/releases/latest)
  [![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
  [![Windows](https://img.shields.io/badge/Windows-10%2F11-0078D6?logo=windows)](https://github.com/opn-build/OpenAlive-Releases/releases/latest)
  [![Languages](https://img.shields.io/badge/languages-8-orange)](#languages)
</div>

---

**OpenAlive** simulates occasional mouse and keyboard activity to prevent idle timeout, keeping your Windows session active without any manual intervention.

> No account. No cloud. No tracking. Runs entirely on your local machine.

## Download

**[⬇ Download OpenAlive\_lasted](https://github.com/opn-build/OpenAlive-Releases/releases/latest)**

*Windows 10 / 11 · No admin rights required · ~21 MB*

---

## Features

- **Mouse simulation** — moves the cursor by a configurable pixel distance at regular intervals
- **Keyboard simulation** — optionally sends a configurable key press (Shift, Ctrl, F13, ScrollLock…)
- **Schedule control** — activate only during work hours, with optional lunch break exclusion
- **System tray** — runs silently in the background; green icon = active, gray = inactive
- **8 languages** — switch live without restarting the app
- **Autostart** — optional Windows startup registration (no admin required)
- **Privacy first** — no telemetry, no network calls, no user accounts
---
<kbd>
<img width="554" height="404" alt="{BFE53D82-A4A6-4A66-93DE-F1C1023C8D91}" src="https://github.com/user-attachments/assets/60f3dfcf-734c-40df-9114-1ea1c8c16499" />

</kbd>
<kbd>
<img width="553" height="431" alt="{774B524F-2C7D-4D0B-AF6C-0A704F221B1B}" src="https://github.com/user-attachments/assets/f48c11a9-3ce2-4b3a-b996-c13cda7bb793" />
</kbd>
<kbd>
<img width="549" height="473" alt="{9B6D558F-B074-4F96-8E14-88CB6D925BA3}" src="https://github.com/user-attachments/assets/8cb792dd-3683-4d88-926d-b5dc6542a864" />
</kbd>

## Installation

1. Download `OpenAlive_Setup_lasted.exe` from the [Releases page](https://github.com/opn-build/OpenAlive-Releases/releases/latest)
2. Run the installer — no administrator rights required
3. OpenAlive installs to `%LOCALAPPDATA%\OpenAlive`

To uninstall: **Control Panel → Programs → OpenAlive → Uninstall**
(removes the Windows startup registry entry automatically)

---

## Languages

| Flag | Language           | Code  |
|------|--------------------|-------|
| 🇪🇸  | Español            | es    |
| 🇺🇸  | English            | en    |
| 🇧🇷  | Português (Brasil) | pt-BR |
| 🇫🇷  | Français           | fr    |
| 🇯🇵  | 日本語              | ja    |
| 🇨🇳  | 中文 (简体)         | zh-CN |
| 🇰🇷  | 한국어              | ko    |
| 🇭🇹  | Kreyòl ayisyen     | ht    |

Switch language from the **Settings** tab — applies immediately, no restart needed.

---

## System Requirements

|               | Minimum                          |
|---------------|----------------------------------|
| OS            | Windows 10 (1903+) or Windows 11 |
| RAM           | ~30 MB at runtime                |
| Disk          | ~25 MB installed                 |
| Rights        | Standard user (no admin)         |

---

## Privacy

OpenAlive runs entirely on your local machine:

- No telemetry
- No data collection
- No cloud services
- No user accounts
- No network requests of any kind

All configuration is stored locally at `%LOCALAPPDATA%\OpenAlive\config.json`.

---

## Built With

**Language**

![Python](https://img.shields.io/badge/Python-3.11-3776AB?logo=python&logoColor=white)

**Libraries & Plugins**

| Package | Version | Purpose |
|---------|---------|---------|
| [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter) | ≥ 5.2 | Modern Tkinter UI — dark/light mode, themed widgets |
| [Pillow (PIL)](https://python-pillow.org) | ≥ 10.0 | Image handling and icon generation |
| [pyautogui](https://pyautogui.readthedocs.io) | ≥ 0.9.54 | Mouse and keyboard simulation |
| [pystray](https://github.com/moses-palmer/pystray) | ≥ 0.19.5 | Windows system tray icon and menu |
| [PyInstaller](https://pyinstaller.org) | ≥ 6.0 | Bundles the app into a standalone `.exe` |
| [ctypes / winreg](https://docs.python.org/3/library/ctypes.html) | stdlib | Windows API — single-instance mutex, autostart registry |
| [Inno Setup 6](https://jrsoftware.org/isinfo.php) | 6.x | Builds the Windows installer |
---

## Support the Project

If OpenAlive is useful to you, consider a small donation via PayPal — it helps keep the project maintained.

[![Donate via PayPal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://paypal.me/fcapuz)

---
