# NTE AutoFish

Windows fishing assistant for NTE: Neverness to Everness.

[![Release](https://img.shields.io/badge/release-v0.1.1-50f0ba)](#latest-update)
[![Platform](https://img.shields.io/badge/platform-Windows-56d8ff)](#recommended-environment)
[![Python](https://img.shields.io/badge/python-3.11%2B-3776ab?logo=python&logoColor=white)](#recommended-environment)
[![Demo](https://img.shields.io/badge/demo-YouTube-ff0000?logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=0h5MJfFbXqk)
[![Buy](https://img.shields.io/badge/buy-LemonSqueezy-7047eb)](https://cilabworks.lemonsqueezy.com/checkout/buy/33197307-b8af-4bfd-b07a-3355cbcce4b6)
[![Support](https://img.shields.io/badge/support-GitHub%20Issues-24292f?logo=github&logoColor=white)](../../issues)
[![License](https://img.shields.io/badge/license-proprietary-lightgrey)](LICENSE.md)
[![Unofficial](https://img.shields.io/badge/status-unofficial-orange)](#disclaimer)

[![Watch the NTE AutoFish demo](assets/nte-autofish-thumbnail.png)](https://www.youtube.com/watch?v=0h5MJfFbXqk)

[Buy / Download on LemonSqueezy](https://cilabworks.lemonsqueezy.com/checkout/buy/33197307-b8af-4bfd-b07a-3355cbcce4b6)
| [itch.io marketplace page](https://ranats.itch.io/nte-autofish)
| [Watch the demo](https://www.youtube.com/watch?v=0h5MJfFbXqk)
| [X / Twitter](https://x.com/PixelUtilityLab/status/2052105671139803640)
| [Japanese guide](README_JA.md)

NTE AutoFish is a small Windows utility that uses screen recognition to assist repeated fishing actions in NTE. It watches the fishing UI and sends keyboard inputs for casting, hook prompts, the fishing bar minigame, and result-screen recovery.

## Latest Update

Current release: `v0.1.1`  
Last updated: 2026-05-10

- Improved result-screen detection and close/retry behavior after a catch.
- Added safer pause behavior when the no-bait notice or fishing menu is detected.
- Reduced false pauses from no-bait detection while the normal cast prompt is visible.
- Improved foreground-window handling so inputs are skipped when the NTE window cannot be confirmed.
- Added target-window capture support when configured.
- Tuned cast/hook retry timing for briefly hidden prompts or missed inputs.

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

Primary checkout:

`https://cilabworks.lemonsqueezy.com/checkout/buy/33197307-b8af-4bfd-b07a-3355cbcce4b6`

Marketplace mirror:

`https://ranats.itch.io/nte-autofish`

LemonSqueezy is the primary direct checkout for this project. The itch.io page is kept as a marketplace presence and alternate download route when available. Payment, receipt, refund, and download-link issues should be handled through the store where you purchased.

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

For payment, receipt, refund, or download-link issues, use the support/contact flow from the store where you purchased.

Do not post private account information, purchase receipts, or UID screenshots publicly.

## Disclaimer

This is an unofficial automation tool. It is not affiliated with Hotta Studio, Perfect World Games, YouTube, GitHub, itch.io, LemonSqueezy, X, or Neverness to Everness.

Automating gameplay may violate game terms of service. Use at your own risk. Operation is not guaranteed after game updates, UI changes, anti-cheat changes, account restrictions, or unsupported display settings.
