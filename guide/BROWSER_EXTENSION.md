# Velocity browser extension

With the extension installed, **clicking a download on any website opens it in Velocity**
instead of the browser's Save dialog, just like other download managers do.

- Works with **Google Chrome, Microsoft Edge, Brave, Opera and Vivaldi** (Windows 10/11).
  Firefox is coming soon.
- Needs **Velocity 0.3.0 or newer**. Velocity updates itself, so you probably have it already.
  Check under Help → About.
- **Sites that need you to be signed in work too.** The extension gives Velocity the cookies for
  that one site, so file hosts that tie links to your browser session download fine.
- If Velocity isn't running, or the link turns out to be a web page (a sign-in page, a captcha,
  a countdown), the browser downloads as usual. Nothing ever gets lost.

---

## Install (Chrome, Edge, Brave, Opera, Vivaldi)

The extension is under review for the Chrome Web Store and Edge Add-ons. Until it's listed
there, install it in one minute like this:

1. **Download** [Velocity-browser-extension.zip](https://github.com/qwertiian/velocity-fast-downloader/releases/latest/download/Velocity-browser-extension.zip).
2. **Unzip it** to a folder you'll keep, for example `Documents\Velocity extension`.
   (Don't delete this folder later; the browser loads the extension from it.)
3. Open the extensions page:
   - Chrome / Brave / Vivaldi: type `chrome://extensions` in the address bar
   - Edge: type `edge://extensions`
   - Opera: type `opera://extensions`
4. Turn on **Developer mode** (top right in Chrome; left side in Edge).
5. Click **Load unpacked** and select the folder from step 2 (the one containing `manifest.json`).
6. Optional: click the puzzle-piece icon in the toolbar and **pin** Velocity.

Click the Velocity icon in the toolbar. It should say **"Connected to Velocity 0.3.0"**.

> Chrome may occasionally show a reminder about developer-mode extensions. That's normal for
> extensions installed this way and goes away once the Chrome Web Store version is out.

## Using it

- **Just click download links** as usual. Velocity's *"Download from browser"* window pops up
  with the file name and size. Click **Download** (or **Later** to add it paused, or **Cancel**).
- **Right-click** any link, image or video → **Download with Velocity**.
- Click the toolbar icon to:
  - switch **Send downloads to Velocity** off temporarily, and
  - **skip small files** (for example, under 500 KB) so they stay in the browser.
- In Velocity: **Tools → Options → General → Take over downloads from my browser** turns the
  feature off on the app side.

## Privacy and security

- The extension talks **only to the Velocity app on your own computer** (address `127.0.0.1`).
  Nothing is sent to us or to anyone else.
- For each download, it gives Velocity the cookies of **that download's site only**, exactly
  what your browser itself would send. Velocity keeps them in memory for the current session
  and **never saves them to disk**.
- Downloads in **private/incognito windows are never touched**.
- Velocity's side only accepts the extension: web pages can't send it downloads.
- Nothing downloads without your click in the Velocity window.

## Troubleshooting

**The popup says "Velocity isn't running".** Start Velocity (it can sit in the notification
area). To have it always ready, turn on *Start Velocity when I sign in* in Options.

**Downloads still go to the browser.**
- Make sure the extension's switch is on and Velocity is 0.3.0 or newer.
- Check *Take over downloads from my browser* in Velocity's Options.
- Downloads created by a web page itself (for example "Export" buttons that build the file in
  your browser) can't be handed over and stay in the browser. That's expected.
- If a site shows a web page instead of the file, Velocity leaves that one to the browser.

**A site's file needs a sign-in and fails in Velocity.** Sign in on the site first, then click
its download button again so the extension can pass on your current session.

**Remove the extension.** Open the extensions page (step 3) and click **Remove**.

---

Questions or problems? [Open an issue](https://github.com/qwertiian/velocity-fast-downloader/issues).
