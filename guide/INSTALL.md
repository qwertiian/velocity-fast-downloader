# Installing Velocity

## Windows 10 / 11

### Standard install (recommended)
1. Download **[Velocity_x64-setup.exe](https://github.com/qwertiian/velocity-fast-downloader/releases/latest/download/Velocity_x64-setup.exe)**.
2. Double-click it. If Windows shows a warning, see [below](#windows-smartscreen-warning).
3. Follow the installer. It installs for your user account only, so no administrator rights
   are needed.
4. Launch **Velocity** from the Start menu.

Requirements: Windows 10 (version 1803+) or Windows 11, 64-bit. The installer adds Microsoft
Edge WebView2 automatically if your PC doesn't have it (it's preinstalled on Windows 11).

### MSI package (IT administrators)
**[Velocity_x64.msi](https://github.com/qwertiian/velocity-fast-downloader/releases/latest/download/Velocity_x64.msi)**
works with Intune, SCCM, Group Policy or `msiexec`:

```bat
msiexec /i Velocity_x64.msi /qn
```

### Windows SmartScreen warning
New apps that aren't yet code-signed show **"Windows protected your PC"**. To continue:
click **More info** → **Run anyway**.

This is a reputation check, not a virus detection. To be sure your file is genuine, compare
its checksum with the one published on the release page:

```powershell
Get-FileHash .\Velocity_x64-setup.exe -Algorithm SHA256
```

The result must match the line for that file in `SHA256SUMS.txt` on the
[release page](https://github.com/qwertiian/velocity-fast-downloader/releases/latest).
Only download Velocity from this GitHub page or the official website.

### Updating
Download and run the newest installer. Your downloads, history and settings are kept.

### Uninstalling
**Settings → Apps → Installed apps → Velocity → Uninstall.**
Your history database stays in `%APPDATA%\dev.velocitydm.desktop\`. Delete that folder too if
you want to remove everything. Files you downloaded are never touched.

## macOS and Linux
Not available yet; they're [coming soon](../README.md#coming-soon).
**Watch** this repository (top right → Watch → Custom → Releases) to be notified.
