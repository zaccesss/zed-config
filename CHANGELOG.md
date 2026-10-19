# Changelog

All notable changes to this project are recorded here.

Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
Versioning follows [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [Unreleased]

## 2026-10-19

### Added

- Initial release: `settings.json` with interface and editor font sizes and a theme that follows
  the system, `High Contrast VSCode` in dark mode and `One Light` in light mode
- `extensions.txt` listing the High Contrast Themes extension the dark theme comes from
- Setup and reference guides with the config folder for macOS, Linux and Windows
- `ACCESSIBILITY.md` with measured contrast ratios for both themes
- CI that parses `settings.json` the way Zed does and checks the extension list

### Changed

- Light mode now uses `Zacess Light` from the Zacess Themes extension instead of `One Light`.
  Every syntax colour now reaches 8.37:1 or more, where most of `One Light`'s fell below 4.5:1
- `settings.json` sets `auto_install_extensions` for `high-contrast-themes` and `zacess-themes`,
  so Zed installs both theme extensions on its own
- `extensions.txt` adds `zacess-themes@0.1.5`
- `ACCESSIBILITY.md` replaces the `One Light` low-contrast warning with measured `Zacess Light`
  figures
- The README and guides name the new theme and the second extension
