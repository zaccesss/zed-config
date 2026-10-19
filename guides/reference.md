# Reference

Every `settings.json` key explained, the extension list and the default key bindings worth
knowing.

## `settings.json`, every key

| Key | Value | Why |
| --- | --- | --- |
| `ui_font_size` | `16` | Zed's own default, pinned so a change to Zed's defaults never shrinks the interface text. |
| `buffer_font_size` | `15` | Zed's own default for editor text, pinned for the same reason. |
| `theme.mode` | `system` | Follows the system's light and dark mode. |
| `theme.dark` | `High Contrast VSCode` | White text on pure black with VS Code's high-contrast syntax colours. Comes from the High Contrast Themes extension, not Zed itself. |
| `theme.light` | `One Light` | Zed's built-in light theme and its default. The High Contrast Themes extension only ships dark themes. |

The comment block at the top of the file is the comment Zed writes into a new settings file, left in place. Zed reads the
file as JSON with comments and trailing commas, so a strict JSON parser rejects it.

## Extensions

| Extension | Version | Why |
| --- | --- | --- |
| `high-contrast-themes` | `0.1.0` | Provides `High Contrast VSCode` and nine other high-contrast dark themes. |

Zed also installs the `html` extension on its own through its default `auto_install_extensions`
setting, so it is not listed.

## Default key bindings worth knowing

There is no custom `keymap.json`, Zed's defaults apply everywhere.

| Action | macOS | Windows and Linux |
| --- | --- | --- |
| Command palette | `Cmd+Shift+P` | `Ctrl+Shift+P` |
| Open settings | `Cmd+,` | `Ctrl+,` |
| Extensions page | `Cmd+Shift+X` | `Ctrl+Shift+X` |
| Theme picker | `Cmd+K` then `Cmd+T` | `Ctrl+K` then `Ctrl+T` |
| Editor text larger or smaller, this session only | `Cmd+=` and `Cmd+-` | `Ctrl+=` and `Ctrl+-` |
