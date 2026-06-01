# Changelog

All notable changes to OpenAlive are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.2] - 2026-05-31

### Changed
- **Faster startup.** The app is now packaged in PyInstaller *onedir* mode
  instead of *onefile*. The single-file build self-extracted the full ~20 MB
  payload to a temporary folder on every launch before any code ran; the
  onedir build skips that step entirely, so the window and tray icon appear
  almost immediately.
- **UPX compression disabled** in the build. UPX-compressed DLLs had to be
  decompressed in memory at every launch (and triggered repeated antivirus
  re-scans of the extracted temp files). Disabling it trades a slightly larger
  install size for a noticeably faster, quieter startup.
- `pyautogui` (and its transitive dependencies: `pyscreeze`, `PIL`,
  `mouseinfo`) is now imported lazily inside the activity worker thread instead
  of at module load, keeping the heavy import off the startup critical path.

### Notes
- No functional or behavioral changes: mouse/keyboard simulation, schedule,
  tray, languages, and autostart all work exactly as before.
- The installer still ships as a single `OpenAlive_Setup_v1.0.2.exe`; the
  onedir layout is internal to the install folder (`%LOCALAPPDATA%\OpenAlive`).

## [1.0.1] - 2026-05-30

- Public release on GitHub (`opn-build/OpenAlive-Releases`).

## [0.0.2] - 2026-05-29

- Early pre-release build.

## [0.0.1] - 2026-05-29

- Initial pre-release build.

[1.0.2]: https://github.com/opn-build/OpenAlive-Releases/releases/tag/v1.0.2
[1.0.1]: https://github.com/opn-build/OpenAlive-Releases/releases/tag/v1.0.1
