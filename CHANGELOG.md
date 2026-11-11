# Changelog

## v0.2.1

- New: **Help → Third-party licences** shows the licences of the open-source components included in Velocity.
- First release delivered through the in-app updater.

## v0.2.0

**New**
- Classic Windows interface: menu bar, toolbar, folder tree, sortable multi-select list,
  right-click menus, block progress bars, tabbed Properties and Options, setup wizard.
- Classic and Classic Dark themes (View menu), or follow Windows.
- Runs in the notification area: closing the window keeps downloading; optional start with Windows.
- Clipboard catcher: copy a download link and Velocity asks whether to download it.
- Automatic, signature-verified updates from inside the app.
- Live download map (per-connection progress) in Properties.
- Detects links that return a web page instead of the file, and explains what to do.

**Security**
- Downloads are tagged as coming from the internet (Mark of the Web), so Windows checks them like browser downloads.
- Downloads can't be saved into Windows system folders.
- The app window is locked to its own content.

**Fixed**
- Light theme couldn't be selected.

## v0.1.0 — First public preview (Windows)

**New**
- Multi-connection downloads with automatic work balancing between connections.
- Pause and resume, including after closing the app, a crash or a restart.
- Automatic retries for dropped connections, stalls and server errors; backs off when a server
  limits connections.
- Protection against corrupted resumes when the file on the server changed.
- Optional SHA-256/SHA-512 verification.
- Overall and per-download speed limits; queue with a limit on simultaneous downloads.
- Automatic categories, search, filters and download statistics.
- Paste-a-link-anywhere, keyboard shortcuts, light/dark themes, notifications.

**Known limitations**
- Windows only for now; macOS and Linux are planned.
- Installers aren't code-signed yet, so Windows shows a SmartScreen warning on first run.
- No browser extension yet: copy and paste links into the app.
