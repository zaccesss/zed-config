# Accessibility

The dark theme puts contrast first and the theme follows the system, so Zed changes with the terminal and the other editors.

> [!NOTE]
> Some of these settings are preferences rather than requirements. Change them freely in your own copy. If a change would help other people too, open an issue or a pull request so I can consider it for everyone.

## Vision

- Dark mode uses `High Contrast VSCode` from the High Contrast Themes extension: white text on pure black at 21:1. Every syntax colour reaches 7:1 or more on the black background except regular expressions (`#d16969`, 5.94:1). Comments are green (`#7ca668`) at 7.51:1.
- Muted interface text (`#a6a6a6`) reaches 8.63:1. Errors (`#f48771`, 8.55:1), warnings (`#cca700`, 9.09:1) and information (`#75beff`, 10.57:1) all stay well above 4.5:1.
- The focused element gets a bright yellow border (`#f8f800`, 18.42:1) and other borders are cyan (`#6fc3df`, 10.55:1), so focus is clear without relying on a subtle shade.
- The current line number is white. Other line numbers are grey (`#6b6b6b`) at 3.94:1, the theme's own choice to keep them quieter than the code.
- Interface text is 16 pixels and editor text 15 pixels. `Cmd+=` and `Cmd+-` (`Ctrl+=` and `Ctrl+-` on Windows and Linux) change the editor text for the current session. Raise `buffer_font_size` and `ui_font_size` in `settings.json` to make it permanent.

> [!WARNING]
> Light mode uses Zed's built-in `One Light`. Body text is `#242529` on `#fafafa` at 14.67:1, but most syntax colours fall below 4.5:1: comments (`#a2a3a7`) are 2.41:1, strings (`#649f57`) 3.03:1, functions (`#5b79e3`) 3.80:1 and keywords (`#a449ab`) 4.88:1. The extension has no light theme. Set `theme.mode` to `dark` in `settings.json` to stay on `High Contrast VSCode` all day.

> [!IMPORTANT]
> `High Contrast VSCode` only exists once the High Contrast Themes extension is installed, see [guides/setup.md](guides/setup.md). Until then dark mode does not get these colours.

## Keyboard

- No custom key bindings yet. Zed's defaults are used on every platform, so its own documentation applies unchanged. The ones worth knowing are in [guides/reference.md](guides/reference.md#default-key-bindings-worth-knowing).
- The theme picker (`Cmd+K` then `Cmd+T`, `Ctrl+K` then `Ctrl+T` on Windows and Linux) switches theme from the keyboard without opening `settings.json`.

## Feedback wanted

If something here gets in the way, open an [issue](https://github.com/zaccesss/zed-config/issues/new/choose) describing what happened and what would work better.

## The shared statement

> [!NOTE]
> I keep one shared accessibility statement for all my projects: [zaccesss/accessibility](https://github.com/zaccesss/accessibility) or on [my site](https://isaacadjei.me/accessibility). This file takes precedence where the two differ.
