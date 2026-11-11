# FAQ & troubleshooting

### Is Velocity really free?
Yes. No price, no ads, no "pro" version, no account.

### Is it safe?
Velocity never runs downloaded files on its own, verifies checksums when you give one, refuses
to resume a file that changed on the server, and contains no tracking. Check that your
installer's SHA-256 matches the release page ([how](INSTALL.md#windows-smartscreen-warning)).

### Why does Windows say "Windows protected your PC"?
The installer isn't code-signed yet (certificates cost money; it's on the roadmap). Click
**More info → Run anyway**.

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
In your download folder (Settings → Download folder). Click **📂** on any row to jump there.
Unfinished files end in `.vpart`. Don't open those; they become the real file when complete.

### Can I download YouTube/Netflix/streaming videos?
No. Velocity downloads direct file links only and doesn't bypass DRM or website restrictions.

### Can it grab downloads from my browser automatically?
Browser extensions for Chrome, Edge and Firefox are next on the roadmap. For now, copy the link
and paste it into Velocity.

### Still stuck?
[Open an issue](https://github.com/qwertiian/velocity-fast-downloader/issues/new?template=bug_report.md)
with your Windows version, Velocity version and the error message. Don't include private links.
