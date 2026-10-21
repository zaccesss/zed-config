# Accessibility

The theme puts contrast first and stays fixed on `Zacess Deep Contrast Dark` until it is changed by hand.

> [!NOTE]
> Some of these settings are preferences rather than requirements. Change them freely in your own copy. If a change would help other people too, open an issue or a pull request so I can consider it for everyone.

## Vision

- The theme is `Zacess Deep Contrast Dark` from the Zacess Themes extension: white text on pure black at 21:1 with deep, fully saturated colours, every syntax colour at 9.0:1 or more. Keywords are blue (`#67aeff`, 9.1:1) and bold, comments green (`#00c600`, 9.1:1) and italic, strings orange (`#ffaa7c`, 11.3:1). The focused element gets a yellow outline and frames are cyan.
- `Zacess Deep Contrast Light`, its light counterpart, is black on white with vivid colours at 7.7:1 or more. It is the `light` theme in `settings.json`, used when `theme.mode` is `light` or `system`.
- All eight Zacess themes, plus the High Contrast Themes extension's dark themes, are in the theme picker. The full measured tables are in the [Zacess Themes accessibility statement](https://github.com/zacesshq/themes/blob/main/ACCESSIBILITY.md).
- Interface text is 16 pixels and editor text 15 pixels. `Cmd+=` and `Cmd+-` (`Ctrl+=` and `Ctrl+-` on Windows and Linux) change the editor text for the current session. Raise `buffer_font_size` and `ui_font_size` in `settings.json` to make it permanent.

> [!IMPORTANT]
> The two Deep Contrast themes only exist once Zacess Themes 0.3.0 or later is installed. `settings.json` lists it under `auto_install_extensions`, so Zed installs it on its own, see [guides/setup.md](guides/setup.md). Until then Zed falls back to its default theme.

## Keyboard

- No custom key bindings yet. Zed's defaults are used on every platform, so its own documentation applies unchanged. The ones worth knowing are in [guides/reference.md](guides/reference.md#default-key-bindings-worth-knowing).
- The theme picker (`Cmd+K` then `Cmd+T`, `Ctrl+K` then `Ctrl+T` on Windows and Linux) switches theme from the keyboard without opening `settings.json`.

## Feedback wanted

If something here gets in the way, open an [issue](https://github.com/zaccesss/zed-config/issues/new/choose) describing what happened and what would work better.

## The shared statement

> [!NOTE]
> I keep one shared accessibility statement for all my projects: [zaccesss/accessibility](https://github.com/zaccesss/accessibility) or on [my site](https://isaacadjei.me/accessibility). This file takes precedence where the two differ.
