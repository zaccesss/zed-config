# Accessibility

Both themes put contrast first and the theme follows the system, so Zed changes with the terminal and the other editors.

> [!NOTE]
> Some of these settings are preferences rather than requirements. Change them freely in your own copy. If a change would help other people too, open an issue or a pull request so I can consider it for everyone.

## Vision

- Dark mode uses `High Contrast VSCode` from the High Contrast Themes extension: white text on pure black at 21:1. Every syntax colour reaches 7:1 or more on the black background except regular expressions (`#d16969`, 5.94:1). Comments are green (`#7ca668`) at 7.51:1.
- Muted interface text (`#a6a6a6`) reaches 8.63:1. Errors (`#f48771`, 8.55:1), warnings (`#cca700`, 9.09:1) and information (`#75beff`, 10.57:1) all stay well above 4.5:1.
- The focused element gets a bright yellow border (`#f8f800`, 18.42:1) and other borders are cyan (`#6fc3df`, 10.55:1), so focus is clear without relying on a subtle shade.
- The current line number is white. Other line numbers are grey (`#6b6b6b`) at 3.94:1, the theme's own choice to keep them quieter than the code.
- Light mode uses `Zacess Light` from the Zacess Themes extension: near-black text (`#111111`) on white at 18.88:1. Every syntax colour reaches 8.37:1 or more, the lowest being comments (`#434f5b`) at 8.37:1. Functions and links (`#0049a3`) are 8.46:1, keywords (`#58099c`) 10.86:1 and strings (`#004a0e`) 10.57:1.
- In light mode muted interface text (`#424242`) is 10.05:1, errors (`#810005`) 10.85:1, warnings (`#583600`) 10.81:1 and information (`#003a84`) 10.83:1. Line numbers (`#4d4d4d`) are 8.45:1 and the focused border (`#0049a3`) 8.46:1.
- Interface text is 16 pixels and editor text 15 pixels. `Cmd+=` and `Cmd+-` (`Ctrl+=` and `Ctrl+-` on Windows and Linux) change the editor text for the current session. Raise `buffer_font_size` and `ui_font_size` in `settings.json` to make it permanent.

> [!IMPORTANT]
> `High Contrast VSCode` and `Zacess Light` only exist once the High Contrast Themes and Zacess Themes extensions are installed. `settings.json` lists both under `auto_install_extensions`, so Zed installs them on its own, see [guides/setup.md](guides/setup.md). Until then the themes do not get these colours.

## Keyboard

- No custom key bindings yet. Zed's defaults are used on every platform, so its own documentation applies unchanged. The ones worth knowing are in [guides/reference.md](guides/reference.md#default-key-bindings-worth-knowing).
- The theme picker (`Cmd+K` then `Cmd+T`, `Ctrl+K` then `Ctrl+T` on Windows and Linux) switches theme from the keyboard without opening `settings.json`.

## Feedback wanted

If something here gets in the way, open an [issue](https://github.com/zaccesss/zed-config/issues/new/choose) describing what happened and what would work better.

## The shared statement

> [!NOTE]
> I keep one shared accessibility statement for all my projects: [zaccesss/accessibility](https://github.com/zaccesss/accessibility) or on [my site](https://isaacadjei.me/accessibility). This file takes precedence where the two differ.
