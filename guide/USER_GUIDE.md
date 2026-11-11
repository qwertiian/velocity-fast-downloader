# How to use Velocity

## 1. First launch
Velocity asks two things: **where to save downloads** (default: your Downloads folder) and your
preferred **theme** (system, light or dark). You can change both later in **Settings**.

## 2. Adding a download
Any of these work:
- **Paste anywhere:** copy a link in your browser, click into Velocity, press **Ctrl + V**.
- **Add button:** click **Add download** (or press **Ctrl + N**) and paste the link.

The add window checks the link and shows:
- the **file name** (you can rename it),
- the **size**,
- a green **"Resumable · multi-connection"** badge when the server allows split downloads.
  A yellow **"Single connection"** badge means the server doesn't, so the file downloads in
  one piece and restarts if interrupted.

Optional settings under **Advanced options**:
- **Connections:** how many parallel connections to use for this file (1–32).
- **Referrer page:** a few sites only allow downloads that come from their own page.
- **Expected checksum:** paste the SHA-256 or SHA-512 a publisher lists. Velocity verifies the
  finished file and warns you if it doesn't match.

Click **Download** to start, or **Add paused** to start it later.

> Velocity needs a **direct link to a file** (one that ends in a download, like `.zip`, `.exe`,
> `.iso`, `.mp4`). Links to a web page or a streaming player won't work.

## 3. Managing downloads
Each row shows progress, speed, time left and active connections (e.g. `8×`).

| Button | What it does |
|---|---|
| ⏸ Pause / ▶ Resume | Stop and continue later, without losing progress |
| ↻ Retry | Try a failed download again (continues where possible) |
| 📂 Show in folder | Opens the folder containing the file |
| ✕ Cancel | Stops the download and deletes the partial file |
| ⋯ More | Properties, copy link, restart from scratch, remove from list, delete file |

**Pause all / Resume all** is the button next to the speed indicator in the top bar.
**Double-click** a finished download to open it. Opening programs (`.exe`, `.msi`…) asks for
confirmation first.

## 4. Lists and categories
The sidebar filters **All**, **Active**, **Queued & paused**, **Completed** and **Failed**.
**Categories** (Videos, Documents, Archives, Applications, Audio, Images, Development) appear
automatically as you download. Use **Ctrl + F** to search by name or link.

## 5. Settings
- **Download folder**, and optionally **sort into category folders** (Videos/, Documents/…).
- **Same-name files:** *Keep both* saves `file (1).zip`; *Replace it* overwrites.
- **Resume interrupted downloads on launch.**
- **Connections per download** (default 8) and **Simultaneous downloads** (default 3; the
  rest wait in the queue).
- **Overall speed limit**, e.g. `2M` = 2 MB/s, `500K` = 500 KB/s. Leave empty for unlimited.
  Individual downloads can also be limited in their **Properties** panel.
- **Compute SHA-256** for every finished download.
- **Notifications** when downloads finish or fail.
- **Theme.**

## 6. Statistics
**Statistics** shows how much you downloaded per day, completed/failed counts and peak speed
for the last 7, 30 or 90 days. It's all stored only on your computer.

## 7. If something goes wrong
See the [FAQ & troubleshooting](FAQ.md).
