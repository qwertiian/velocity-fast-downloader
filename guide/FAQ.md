# FAQ & troubleshooting

### Is Velocity really free?
Yes. No price, no ads, no "pro" version, no account.

### Where should I download it from?
The **[Microsoft Store](https://apps.microsoft.com/detail/9NGHWBDW4TGB)** is recommended: one-click install, signed by
Microsoft and automatic updates. The direct installer on the GitHub Releases page is the same app.

### I pasted a link to a .zip/.rar but Velocity says it's a web page
The site only gives the file to your browser (sign-in, captcha, countdown or a session cookie).
Start the download in your browser, then copy the real link from the browser's Downloads list
(**Ctrl + J** → right-click → *Copy download link*) and paste it into Velocity. Easier: install the
[browser extension](BROWSER_EXTENSION.md), click the site's download button, and Velocity takes
over with your session (works for hosts that need you to be signed in).

### I closed the window. Is Velocity still running?
Yes, if *Keep running in the notification area* is on (the default). Downloads continue. Click
the Velocity icon next to the clock to reopen it, or right-click it → **Exit Velocity** to quit.

### How do updates work?
Velocity checks for new versions on launch (switchable in Options → Updates & privacy) and
shows **Install and restart**. Updates come only from the official releases and are installed
only if their digital signature is valid.

### The "Download this file?" window keeps popping up
It appears when you copy a link to a file. Tick **Don't ask again** in it, or switch off
*Offer to download links I copy* in **Tools → Options → General** (or the Tools menu).

### Is it safe?
Velocity never runs downloaded files on its own, verifies checksums when you give one, refuses
to resume a file that changed on the server, and contains no tracking. Check that your
installer's SHA-256 matches the release page ([how](INSTALL.md#windows-smartscreen-warning)).

### Why does Windows say "Windows protected your PC"?
That only happens with the direct installer from GitHub, which isn't code-signed yet. Click
**More info → Run anyway**, or install Velocity from the
[Microsoft Store](https://apps.microsoft.com/detail/9NGHWBDW4TGB) instead. It's signed by Microsoft and never shows this warning.

### Will it make every download faster?
Not always. Parallel connections help with distant, busy or per-connection-limited servers.
If one connection already uses your full internet speed, more connections can't add speed.

### Why does a download say "Single connection"?
The server doesn't support partial downloads. The file still downloads, but in one piece, and
an interruption means starting that file over.

### "The file on the server changed since this download started"
The publisher replaced the file. Velocity won't mix old and new data, which would corrupt it.
Choose **⋯ → Restart from scratch**.

### "Access denied (HTTP 403)" or "The link may have expired"
Many sites use temporary links. Go back to the website, start the download again, and copy the
fresh link. Some sites also require the **Referrer page** (Advanced options).

### "The server is limiting how fast you can download (429)"
Velocity already reduces connections automatically. If it keeps happening, lower
**Connections per download** in Settings, or try later.

### A download is stuck at "Retrying"
Velocity retries network errors automatically with increasing waits. If it fails in the end,
press **Retry**. Your progress is kept.

### "Couldn't write the file to disk"
Usually the disk is full or the folder isn't writable. Free some space or choose another
folder, then press **Retry**. Progress is kept.

### Where are my files?
In your download folder (**Tools → Options → Save to**). Right-click any download → **Open folder** to jump there.
Unfinished files end in `.vpart`. Don't open those; they become the real file when complete.

### Can I download YouTube/Netflix/streaming videos?
No. Velocity downloads direct file links only and doesn't bypass DRM or website restrictions.

### Can it grab downloads from my browser automatically?
Yes. Install the **[Velocity browser extension](BROWSER_EXTENSION.md)** and every download you
click in Chrome or Edge opens in Velocity instead of the browser's Save dialog. If Velocity isn't
running, the browser downloads as usual.

### Can Velocity make Steam or Epic Games downloads faster?
No, and no other download manager can either. Steam and the Epic Games Launcher don't download
games as normal web links. They fetch thousands of small encrypted chunks over their own
signed-in protocol and already use many connections at once. A separate app can't take those
downloads over without your account login and the games' decryption keys, which would break
their terms of service and risk your account.

What actually helps:
- **Steam:** Settings → Downloads → change **Download Region** to a nearby, less busy server
  (try two or three), make sure **Limit bandwidth** is off, and turn off *Throttle downloads
  while streaming*. Clearing the download cache (same page) fixes stuck or slow downloads.
- **Epic Games Launcher:** Settings → turn off *Throttle downloads*. Pause and resume a slow
  download to get a different server.
- **Both:** use a wired connection, install to an SSD (slow disks are often the real limit,
  shown as high disk use in Task Manager), and pause other downloads and streams.

Velocity speeds up regular downloads from websites: installers, ISOs, archives, videos and
files from file hosts.

### Still stuck?
[Open an issue](https://github.com/qwertiian/velocity-fast-downloader/issues/new?template=bug_report.md)
with your Windows version, Velocity version and the error message. Don't include private links.
