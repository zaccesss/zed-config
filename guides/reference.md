# Reference

Every `settings.json` key explained, the extension list and the default key bindings worth
knowing.

## `settings.json`, every key

| Key | Value | Why |
| --- | --- | --- |
| `ui_font_size` | `16` | Zed's own default, pinned so a change to Zed's defaults never shrinks the interface text. |
| `buffer_font_size` | `15` | Zed's own default for editor text, pinned for the same reason. |
| `auto_install_extensions` | `high-contrast-themes` and `zacess-themes` set to `true` | Zed installs both theme extensions on its own, so a new machine gets both themes without a manual step. |
| `theme.mode` | `dark` | The theme stays on `theme.dark` whatever the system appearance. `system` follows light and dark mode with the pair below and `light` fixes the light theme. |
| `theme.dark` | `Zacess Deep Contrast Dark` | White text on pure black at 21:1 with deep, fully saturated colours at 9.0:1 or more. Comes from the Zacess Themes extension, not Zed itself. |
| `theme.light` | `Zacess Deep Contrast Light` | Black on white at 21:1 with vivid colours at 7.7:1 or more, the light counterpart. Comes from the Zacess Themes extension, not Zed itself. |
| `terminal.font_family` | `GeistMono Nerd Font` | The built-in terminal draws the Nerd Font symbols a themed prompt uses (branch, status and battery icons). The font is free under the SIL Open Font License and must be installed first, from the [Nerd Fonts releases](https://github.com/ryanoasis/nerd-fonts/releases). The buffer font is unchanged. |

The comment block at the top of the file is the comment Zed writes into a new settings file, left in place. Zed reads the
file as JSON with comments and trailing commas, so a strict JSON parser rejects it.

## Extensions

| Extension | Version | Why |
| --- | --- | --- |
| `high-contrast-themes` | `0.1.0` | Adds `High Contrast VSCode` and nine other high-contrast dark themes to the picker. Not used by default. |
| `zacess-themes` | `0.3.0` | Provides all eight Zacess themes, the two Deep Contrast themes among them. |

Zed also installs the `html` extension on its own through its default `auto_install_extensions`
setting, which Zed merges with the two entries here, so it is not listed.

## Default key bindings worth knowing

There is no custom `keymap.json`, Zed's defaults apply everywhere.

| Action | macOS | Windows and Linux |
| --- | --- | --- |
| Command palette | `Cmd+Shift+P` | `Ctrl+Shift+P` |
| Open settings | `Cmd+,` | `Ctrl+,` |
| Extensions page | `Cmd+Shift+X` | `Ctrl+Shift+X` |
| Theme picker | `Cmd+K` then `Cmd+T` | `Ctrl+K` then `Ctrl+T` |
| Editor text larger or smaller, this session only | `Cmd+=` and `Cmd+-` | `Ctrl+=` and `Ctrl+-` |
