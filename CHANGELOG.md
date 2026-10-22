# Changelog

All notable changes to this project are recorded here.

Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
Versioning follows [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [Unreleased]

## [0.0.1] - 2026-10-22

### Added

- The built-in terminal uses `GeistMono Nerd Font` (`terminal.font_family`), so Nerd Font prompt symbols draw. The font is free and must be installed from the Nerd Fonts releases; `guides/reference.md` links it. The buffer font is unchanged.

### Changed

- The theme is now fixed on `Zacess Deep Contrast Dark` (`theme.mode` `dark`) with `Zacess Deep Contrast Light` as the light theme, from Zacess Themes 0.3.0, in place of `High Contrast VSCode` and `Zacess Light` following the system. `extensions.txt` records `zacess-themes@0.3.0`. All eight Zacess themes are in the picker.

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
