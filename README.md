# NotchWin

A notch for the top of your Windows screen. A small pill shows the time and battery; hover it for quick
pages, open it for a full workspace. Smooth, true-black, and light on your PC.

**Download:** the latest `notchwin.exe` is on the [Releases](../../releases/latest) page.
**Buy a license:** [NotchWin on Gumroad](https://bhoominn.gumroad.com/l/bkuad)

## Install

1. Download `notchwin.exe` from [Releases](../../releases/latest).
2. Create the folder `%LOCALAPPDATA%\Programs\NotchWin` (paste that into the File Explorer address bar)
   and put `notchwin.exe` in it.
3. Double-click it. The notch appears at the top of your screen and a tray icon is added.
4. Open the Deck (see below) and paste your license key.

Put it in that folder if you want automatic updates: only the copy in `%LOCALAPPDATA%\Programs\NotchWin`
updates itself. No administrator rights are needed. Windows may show a SmartScreen warning the first time
because the app is new; choose **More info > Run anyway**.

Requires Windows 10 or 11.

## Using it

| What | How |
|---|---|
| **Pill** | Always there: the clock in the middle, your battery on the left, music bars or an alert on the right when there is something to show. |
| **Glance** | Hover the pill. Scroll the mouse wheel (or swipe sideways) to change pages. Moving away closes it. |
| **Deck** | Click the button in the Glance header, press <kbd>Win</kbd> + <kbd>`</kbd>, or click the tray icon. <kbd>Esc</kbd> or a click outside closes it. |
| **Menu** | Right-click the notch or the tray icon. |

If <kbd>Win</kbd> + <kbd>`</kbd> is taken by another program, use <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>N</kbd>.

## What it does

- **Clipboard history:** text, links, code and images you copy, searchable, click to copy back. Items that
  password managers mark private are never recorded, and you can pause recording from the menu.
- **File shelf:** drag files onto the notch to park them, drag them out to any app later.
- **Tray tab:** every shelved file in one grid, with image tools right on the tile:
  - **Convert** an image between PNG, JPG and BMP (the original is never changed).
  - **Compress** a PNG or JPG without changing a single pixel (**Exact**), or shrink a PNG much further with
    **Tiny**, which reduces its colours the way TinyPNG does. The result is saved as a new file next to the original.
- **Music:** controls, album art, progress and synced lyrics for whatever is playing in Windows.
- **Alerts on the pill:** volume, brightness, Caps Lock, charger, battery, network and Bluetooth, plus your
  Windows notifications (shown in the Deck's Alerts tab).
- **AI usage:** how much of your Claude, Codex, Cursor and Grok limits you have left, and a click to open each app.
- **To-do list, focus timer and a water reminder.** The focus timer is a Pomodoro with focus, short break and
  long break; it waits for you when time is up.
- **Calendar:** a month view with public holidays for your country (chosen in **Deck > Settings > Calendar**).
- **Clock and world clock:** several clock styles, and up to 8 cities.
- **System:** live CPU and RAM usage, and a **RAM cleaner** button that gives back unused memory (it never closes anything).
- **Dev tab:** a calculator and developer tools, all running on your PC (nothing you type is sent anywhere or stored).
  - **Calculator:** a keypad with a live answer, brackets, square root, powers, sin, cos, tan, logs, memory keys
    and a history you can click to bring a sum back. Percent works like a real calculator (`200 + 10%` is 220).
    You can also just type on your keyboard.
  - **JSON** (format or minify), **Base64** and **URL** (encode or decode), **JWT** (read the header and
    payload and see when it expires), **UUID** (a fresh random one) and **Hash** (MD5, SHA-1, SHA-256, SHA-512).
- **GitHub, Vercel and Cloudflare status**, in the same Dev tab. Connect each one by creating a token on its
  website and pasting it (the Dev tab links to the right page and lists the permissions to give):
  - **GitHub:** your most recently pushed repositories with their open pull requests and whether CI is passing,
    and your activity over the last 30 days. Click a repository to open it.
  - **Vercel:** the latest deployment of each of your projects, and whether it is ready, building or failed.
  - **Cloudflare:** the same for your Cloudflare Pages projects.
- **Status dot and failure alerts:** a dot on the pill is red when something is failing, amber while a build or
  deployment is running and green when everything passes (it shows only while one of these is connected), and the
  pill tells you when a repository's CI or a deployment starts failing.
- **Background checks:** while a service is connected, NotchWin reads it every 10 minutes so the dot and the
  alerts stay current. Turn this off in **Deck > Settings > General > Background checks**; the dot and alerts
  then update only when you open the Glance or the Dev tab.
- **Stays out of the way:** it hides while a fullscreen app or game is in front, and fades away over
  browser tabs at the top of the screen until you pause on the top edge.

**Your own shortcuts:** in **Deck > Settings > Shortcuts**, give any Deck tab its own keyboard shortcut (for
example Ctrl + Alt + M for Media) and it opens straight to that tab from anywhere; press it again to close.
If another program already uses a combination, NotchWin tells you and keeps the old one.

Everything can be arranged in **Deck > Settings**: hide, show and reorder pages, tabs and cards, change the
clock, sleep and glow delays, and more. You can also pick the monitor and the gap from the top edge from the
right-click menu.

## License

NotchWin needs a license key from Gumroad. Open the Deck, click **Paste**, and the key is activated for this
PC. To move NotchWin to another PC, use **Deck > Settings > License > Remove from this PC** first (or "Move it
here" on the new PC, up to 2 moves a month). Lost your key? Find it in your [Gumroad library](https://gumroad.com/library).

One key works on one PC at a time. NotchWin checks the license quietly once a day and keeps working offline
for up to 14 days; after that it asks you to reconnect. Keep your PC's date and time correct: if the clock is
set back, NotchWin locks until it is right again.

## Updates

NotchWin checks for a newer version about 45 seconds after it starts and then once a day. A new version is
downloaded, verified and swapped in quietly; it takes effect the next time NotchWin starts. Nothing
interrupts you.

- Check by hand: **Deck > Settings > License > Check for updates**, or right-click > **Check for updates now**.
- Turn it off: right-click > untick **Update automatically**.
- Or download the newest `notchwin.exe` from [Releases](../../releases/latest) and replace the old one
  (quit NotchWin first from the right-click menu).

## Privacy

NotchWin keeps your data on your PC. Clipboard history, to-dos and the license are stored encrypted for your
Windows account only. It connects to the internet only to:

- check and renew your license, and look for updates;
- fetch song lyrics (title, artist, album and length only, from lrclib.net);
- read your AI usage from each tool's own service, using the sign-in that tool already has (never stored or sent anywhere else);
- read your GitHub, Vercel or Cloudflare status from `api.github.com`, `api.vercel.com` or
  `api.cloudflare.com`, but only for a service you connect. The token you paste is checked with that service,
  kept only if it is accepted, stored encrypted for your Windows account only, and sent to that service and
  nowhere else. **Deck > Dev > Disconnect** deletes it.

It does not log your keys or tokens, and it uses no keyboard hook.

## Start with Windows / quit / uninstall

- **Start with Windows:** right-click > **Start with Windows**.
- **Quit:** right-click > **Quit NotchWin**.
- **Uninstall:** turn off *Start with Windows*, quit, then delete `%LOCALAPPDATA%\Programs\NotchWin`.
  Settings and data live in `%APPDATA%\NotchWin` and `%LOCALAPPDATA%\NotchWin`; delete them too for a clean removal.

## Help

If something does nothing, the log at `%LOCALAPPDATA%\NotchWin\debug.log` usually says why. Email
[bhoominn@gmail.com](mailto:bhoominn@gmail.com?subject=NotchWin) and include the last few lines of it.
