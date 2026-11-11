# Changelog

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
