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
- **Music:** controls, album art, progress and synced lyrics for whatever is playing in Windows.
- **Alerts on the pill:** volume, brightness, Caps Lock, charger, battery, network and Bluetooth, plus your
  Windows notifications (shown in the Deck's Alerts tab).
- **AI usage:** how much of your Claude, Codex, Cursor and Grok limits you have left, and a click to open each app.
- **To-do list, focus timer (Pomodoro) and a water reminder.**
- **Clock and world clock:** several clock styles, and up to 8 cities.
- **System:** live CPU and RAM, and a button that gives back unused memory.
- **Stays out of the way:** it hides while a fullscreen app or game is in front, and fades away over
  browser tabs at the top of the screen until you pause on the top edge.

Everything can be arranged in **Deck > Settings**: hide, show and reorder pages, tabs and cards, change the
clock, sleep and glow delays, and more. You can also pick the monitor and the gap from the top edge from the
right-click menu.

## License

NotchWin needs a license key from Gumroad. Open the Deck, click **Paste**, and the key is activated for this
PC. To move NotchWin to another PC, use **Deck > Settings > License > Remove from this PC** first (or "Move it
here" on the new PC). Lost your key? Find it in your [Gumroad library](https://gumroad.com/library).

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

- check and renew your license, and look for updates (`notchwin.vercel.app`);
- fetch song lyrics (title, artist, album and length only, from lrclib.net);
- read your AI usage from each tool's own service, using the sign-in that tool already has (never stored or sent anywhere else).

It does not log your keys, and it uses no keyboard hook.

## Start with Windows / quit / uninstall

- **Start with Windows:** right-click > **Start with Windows**.
- **Quit:** right-click > **Quit NotchWin**.
- **Uninstall:** turn off *Start with Windows*, quit, then delete `%LOCALAPPDATA%\Programs\NotchWin`.
  Settings and data live in `%APPDATA%\NotchWin` and `%LOCALAPPDATA%\NotchWin`; delete them too for a clean removal.

## Help

If something does nothing, the log at `%LOCALAPPDATA%\NotchWin\debug.log` usually says why. Email
[bhoominn@gmail.com](mailto:bhoominn@gmail.com?subject=NotchWin) and include the last few lines of it.
