# How to use Velocity

## 1. First launch
A short setup wizard asks:
- **where to save downloads** (default: your Downloads folder),
- whether Velocity should **offer to download links you copy**,
- whether it should **keep running in the notification area** and **start with Windows**,
- whether to **check for updates automatically**,
- your **colour scheme**: *Classic*, *Classic Dark* or *Follow Windows*.

Everything can be changed later in **Tools → Options**.

## 2. The main window
- **Menu bar:** File, Downloads, View, Tools, Help.
- **Toolbar:** Add URL, Resume, Pause, Stop, Remove, Resume all, Pause all, Options, Statistics.
- **Folder tree (left):** *All downloads* with Downloading / Queued & paused / Completed /
  Failed & cancelled, plus **Categories** (Video, Music, Compressed, Programs…).
- **Download list (right):** click column headers to sort. Ctrl+click or Shift+click selects
  several downloads. Right-click for every action.
- **Status bar:** what's selected, active downloads, total speed, speed limit and whether the
  clipboard catcher is on.
- **Find box (top right):** filters the list by name or address.

## 3. Adding a download
- **Click it in your browser:** with the [Velocity browser extension](BROWSER_EXTENSION.md),
  clicking any download link opens Velocity's **"Download from browser"** window instead of the
  browser's Save dialog. You can also right-click a link → **Download with Velocity**.
- **Copy a link:** in your browser, right-click a download link → *Copy link address*.
  A small **"Download this file?"** window appears near the clock. Choose **Download**,
  **Later** (adds it paused) or **Ignore**.
- **Add URL:** click **Add URL** (or press **Ctrl + N**) and paste the address.
- **Paste anywhere:** click into the Velocity window and press **Ctrl + V**.

The Add URL window checks the link and shows the file name, size and whether the server
supports **resume and multiple connections**. Under **More options** you can set connections
(1–32), a referrer page some sites require, and an expected **SHA-256/512 checksum** to verify
the finished file.

### "This link opened a web page, not a file"
Some sites only hand out the file to your browser: you must be signed in, solve a captcha or
wait for a countdown. Click the download button on the website, and when the real download
starts, copy its link from your browser's Downloads list (**Ctrl + J** → right-click → *Copy
download link*) and paste it into Velocity. Some file hosts tie even that link to your browser
session: with the [browser extension](BROWSER_EXTENSION.md), just click the site's download
button and Velocity takes over with your session.

## 4. Managing downloads

| Action | How |
|---|---|
| Pause / Resume | Toolbar, right-click, or **Space** |
| Stop (discard partial file) | Toolbar **Stop** (asks first, and offers *Pause instead*) |
| Retry a failed download | **Resume**: continues where it stopped when possible |
| Restart from the beginning | Right-click → *Restart from beginning* |
| Open file / folder | Double-click, **Enter**, or right-click → *Open folder* |
| Remove from list | **Delete** (the file stays on disk) |
| Delete the file from disk | Right-click → *Delete file from disk…* (asks first) |
| Properties | **Alt + Enter** or right-click → *Properties* |

**Properties** has three tabs: *General* (status, address, where it's saved, checksum),
*Connections* (a live **download map** showing each connection's part of the file) and
*Options* (a speed limit for just this download).

Opening a program (`.exe`, `.msi`…) always asks for confirmation. Downloaded files are tagged
as coming from the internet, so Windows checks them just as it does browser downloads.

## 5. Working in the background
With *Keep running in the notification area* on (the default), closing the window **doesn't**
stop downloads. Velocity stays next to the clock:
- **click** the icon to reopen the window,
- **right-click** it for *Pause all*, *Resume all* and **Exit Velocity**,
- **hover** over it to see what's downloading.

To quit completely, use **File → Exit** or *Exit Velocity* in the tray menu.

## 6. Options (Tools → Options)
- **General:** clipboard catcher, notification area, start with Windows, resume on launch,
  notifications.
- **Save to:** download folder, subfolders by type, what to do with same-name files, SHA-256
  for every download.
- **Connection:** connections per download, simultaneous downloads (others wait in the
  queue), overall **speed limit** in KB/s.
- **Appearance:** Classic, Classic Dark, or follow Windows.
- **Updates & privacy:** automatic update checks and a **Check now** button.

## 7. Updates
When a new version is available, Velocity shows what's new and offers **Install and
restart**. Your downloads are paused and saved first, and they continue after the restart.
Updates install only if their digital signature is valid. You can also use **Help → Check for
updates**.

## 8. Statistics
**Statistics** (toolbar or View menu) shows data downloaded per day and completed/failed counts
for the last 7, 30 or 90 days. It's all stored only on your computer.

## 9. Problems?
See the [FAQ & troubleshooting](FAQ.md).
