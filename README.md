# steam_export

Easily export your owned Steam games and manifests into `.rar` files with a simple CLI.

## Features

* **Account Switcher:** Automatically restarts Steam and prompts the account selector so you can pick the exact profile you want to inspect.
* **Interactive Arrow-Key Menus:** Navigate smoothly through your **Installed Library** and **Not Installed Library** using your Up/Down arrow keys and `Enter`—with zero terminal flicker.
* **One-Click `.rar` Export:** Packs your selected installed game folder and its corresponding `appmanifest_*.acf` file into a clean `<Game Name>/<Game Name>.rar` archive in your current working directory.
* **Live Progress Display:** Shows a clean, single-line percentage progress indicator while WinRAR compresses the files.
* **Quick Install Trigger:** Selecting a game from your **Not Installed Library** launches Steam's native installation prompt for that title.
* **Zero External Dependencies:** Built using only Python's standard library.

## Requirements

* **OS:** Windows 10 / Windows 11
* **Python:** Python 3.8 or higher
* **Archiver:** WinRAR installed in its default directory (`C:\Program Files\WinRAR\Rar.exe` or `C:\Program Files (x86)\WinRAR\Rar.exe`)
* **Steam:** Installed locally on your PC

## Download & Installation

1. Go to the **[Releases](../../releases/latest)** page on the right side of this repository and download the latest `steam_export.zip`.
2. Extract the `.zip` archive to any folder.
3. Double-click **`install.bat`** to automatically copy `steam_export.py` and `steam_export.bat` to your user directory and add `steam_export` to your Windows `PATH`.
4. Restart any open terminal windows so the updated `PATH` takes effect.

## Usage

1. Open Command Prompt (`cmd`), PowerShell, or Windows Terminal inside the folder where you want your exported `.rar` archive saved.
2. Run:

```bash
steam_export
```

3. Select your account when the Steam window opens.
4. Use the **Up / Down arrow keys** and press **Enter** to choose between your **Installed library** and **Not installed library**.
5. Pick a game and wait until the terminal displays `Exporting Done`.

> [!WARNING]
> This tool only archives local game files that you own and already have installed via Steam. It does not bypass Steam DRM or download games directly from Valve's servers.

## License

This project is open-source and available under the [MIT License](LICENSE).
