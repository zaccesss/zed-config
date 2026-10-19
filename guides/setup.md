# Setup

## 1. Clone

```bash
git clone https://github.com/zaccesss/zed-config.git ~/.zed-config-src
```

## 2. Find your config folder

| Platform | Config folder |
| --- | --- |
| macOS | `~/.config/zed/` |
| Linux | `~/.config/zed/` (`$XDG_CONFIG_HOME/zed/` when that variable is set) |
| Windows | `%APPDATA%\Zed\` |

Zed creates the folder on first launch. The commands below also create it when Zed has not run
yet.

## 3. Copy the settings into place

macOS and Linux:

```bash
mkdir -p ~/.config/zed
cp ~/.zed-config-src/settings.json ~/.config/zed/settings.json
```

Windows (PowerShell):

```powershell
New-Item -ItemType Directory -Force "$env:APPDATA\Zed" | Out-Null
Copy-Item "$HOME\.zed-config-src\settings.json" "$env:APPDATA\Zed\settings.json"
```

> [!WARNING]
> This overwrites the existing `settings.json`. Back up the old file first if it has settings
> worth keeping.

## 4. Install the extensions

`settings.json` lists both theme extensions under `auto_install_extensions`, so Zed installs
High Contrast Themes and Zacess Themes on its own the next time it starts with this file. To install
them by hand instead, open the Extensions page with `Cmd+Shift+X` on macOS (`Ctrl+Shift+X` on
Windows and Linux), search for **High Contrast Themes** and **Zacess Themes** and install both.
Zed always installs the latest version, the versions in `extensions.txt` only record the ones this
config was last checked against.

## Verify it worked

1. Switch the system to dark mode. Zed should show black backgrounds with white text
   (`High Contrast VSCode`).
2. Switch the system to light mode. Zed should change to `Zacess Light` on its own.
3. Open the theme picker with `Cmd+K` then `Cmd+T` (`Ctrl+K` then `Ctrl+T` on Windows and Linux)
   to confirm both theme names exist.

## Updating after a change to this repo

```bash
cd ~/.zed-config-src
git pull
```

Then repeat the copy step in section 3. Zed picks up a new `settings.json` straight away, no
restart needed.
