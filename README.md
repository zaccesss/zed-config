# zed-config

> Zed editor settings: a high-contrast dark theme that follows the system appearance, the theme
> extension it needs and setup guides for macOS, Linux and Windows.

## What's here

- [`settings.json`](settings.json) - interface and editor font sizes and a theme that follows the
  system: `High Contrast VSCode` in dark mode, `Zacess Light` in light mode, plus
  `auto_install_extensions` so Zed installs both theme extensions on its own. Identical on every
  platform.
- [`extensions.txt`](extensions.txt) - the two extensions the dark and light themes come from,
  one `id@version` per line.

## Setup

Full walkthrough in [guides/setup.md](guides/setup.md): copy `settings.json` into Zed's config
folder and Zed installs the extensions on its own.

> [!IMPORTANT]
> `High Contrast VSCode` and `Zacess Light` are not built into Zed. Until the High Contrast Themes
> and Zacess Themes extensions are installed, the themes do not apply.

## Structure

| Path | Contents |
| --- | --- |
| [`ACCESSIBILITY.md`](ACCESSIBILITY.md) | Measured contrast for the dark and light themes and the font sizes |
| [`settings.json`](settings.json) | Installs to `~/.config/zed/` on macOS and Linux, `%APPDATA%\Zed\` on Windows |
| [`guides/`](guides/) | Setup walkthrough and settings reference |
