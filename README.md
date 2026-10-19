# zed-config

> Zed editor settings: a high-contrast dark theme that follows the system appearance, the theme
> extension it needs and setup guides for macOS, Linux and Windows.

## What's here

- [`settings.json`](settings.json) - interface and editor font sizes and a theme that follows the
  system: `High Contrast VSCode` in dark mode, `One Light` in light mode. Identical on every
  platform.
- [`extensions.txt`](extensions.txt) - the extension the dark theme comes from, one
  `id@version` per line.

## Setup

Full walkthrough in [guides/setup.md](guides/setup.md): copy `settings.json` into Zed's config
folder, then install the extension.

> [!IMPORTANT]
> `High Contrast VSCode` is not built into Zed. Until the High Contrast Themes extension is
> installed, dark mode does not use it.

## Structure

| Path | Contents |
| --- | --- |
| [`ACCESSIBILITY.md`](ACCESSIBILITY.md) | The high-contrast dark theme, the light theme's lower syntax contrast and the font sizes |
| [`settings.json`](settings.json) | Installs to `~/.config/zed/` on macOS and Linux, `%APPDATA%\Zed\` on Windows |
| [`guides/`](guides/) | Setup walkthrough and settings reference |
