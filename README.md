# NTE AutoFish

Windows fishing assistant for NTE: Neverness to Everness.

![NTE AutoFish thumbnail](assets/nte-autofish-thumbnail.png)

[Buy / Download NTE AutoFish](https://cilabworks.lemonsqueezy.com/checkout/buy/33197307-b8af-4bfd-b07a-3355cbcce4b6)
| [Watch the demo](https://youtu.be/0h5MJfFbXqk)
| [Japanese guide](README_JA.md)

NTE AutoFish is a small Windows utility that uses screen recognition to assist repeated fishing actions in NTE. It watches the fishing UI and sends keyboard inputs for casting, hook prompts, the fishing bar minigame, and result-screen recovery.

## What It Does

- Casts from the fishing-ready screen where pressing `F` manually would cast the rod.
- Presses `F` when the fish-hook prompt appears.
- Uses short `A` / `D` inputs to keep the yellow marker near the safe line during the fishing minigame.
- Closes the result screen and returns to the next cast.
- Stops when it detects no bait or a fishing menu state.
- Includes a dry-run mode for detection-only checks before sending live inputs.

## Recommended Environment

- Windows 10/11
- Python 3.11 or later
- NTE in borderless fullscreen mode
- 1920x1080 or higher resolution
- Windows display scale at 100%
- HDR and color filters disabled

If NTE requires administrator-level input on your PC, run PowerShell or Command Prompt as administrator too.

## Before You Buy

This is a Python-based Windows tool, not a standalone mobile app. The program is designed to be started while NTE is already at a fishing spot in the fishing-ready state.

Compatibility can depend on resolution, UI scale, display mode, HDR settings, game updates, anti-cheat behavior, and account environment. Please watch the demo and check the recommended environment before purchasing.

## After Purchase

The release ZIP includes:

- `install.bat`
- `dry_run.bat`
- `run.bat`
- English and Japanese start guides
- `settings.json` for tuning

Typical flow:

```powershell
install.bat
dry_run.bat
run.bat
```

For manual command-line use after setup:

```powershell
python -m nte_autofish run --config .\settings.json
```

Stop the program with `Ctrl+C`.

## Support

For setup issues, open a GitHub issue in this repository and include:

- Windows version
- Python version
- Screen resolution and display scale
- Whether NTE is running in borderless fullscreen
- A short description of where the automation stops

Do not post private account information, purchase receipts, or UID screenshots publicly.

## Disclaimer

This is an unofficial automation tool. It is not affiliated with Hotta Studio, Perfect World Games, YouTube, GitHub, LemonSqueezy, or Neverness to Everness.

Automating gameplay may violate game terms of service. Use at your own risk.
