# Claude-Generated-Windows-12# Windows 12 (Concept)

A fan-made **Windows 12 concept desktop that runs entirely in your browser** — boot screen, lock screen, desktop, windows, taskbar, Start menu, working apps, a fake-internet browser, and a collection of harmless joke "viruses." It's all one self-contained HTML file: no build step, no dependencies, no server.

> ⚠️ This is a hobby/concept project. It is **not affiliated with, endorsed by, or made by Microsoft**. "Windows" and related marks belong to their respective owners.

## ✨ Features

- **Full desktop environment** — draggable/resizable/maximizable windows, a working taskbar, Start menu with search, quick settings, and a calendar.
- **Four themes** — Windows 12 (default), Windows Classic (2000-style), Windows Blue (XP-style), and Windows Aero (7-style). Switchable live.
- **Customization** — drag desktop icons anywhere, create shortcuts, pin/unpin & reorder taskbar and Start items, upload your own wallpaper, set a profile picture, and add a sign-in password.
- **Built-in apps:**
  - **File Explorer** — a persistent virtual C:\ drive with create/rename/delete and a Recycle Bin
  - **Word, Excel, PowerPoint** — a formatting editor, a spreadsheet with real formulas (`=SUM`, `=A1*B2`, …), and a slide editor with Present mode
  - **Horizon** — a pretend web browser that generates a page for any address (no real internet)
  - **Command Prompt** — ~25 commands (`dir`, `cd`, `tree`, `ping`, `tasklist`, `shutdown`, …)
  - **Task Manager** — process list + live CPU/memory graphs
  - **Control Panel, Calculator, Paint, Photos, Notepad, Sticky Notes, Clock, Snake, Minesweeper**
  - **Assistant (Aria)** — an on-device helper that answers questions about the OS and performs actions
- **wvs.net** — a hidden in-browser "virus" site (type `wvs.net` in Horizon). Every "virus" is a **fake, harmless joke** that only affects the simulated OS; a restart cures everything.
- **Saves your state** in the browser (files, settings, layout) via `localStorage`.

## 🚀 Getting started

No installation needed.

1. Download **`index.html`**.
2. Open it in any modern browser (Chrome, Edge, Firefox, Safari).

That's it. To edit, open the same file in any text editor.

## 🖥️ Running locally (optional)

Serving over a local server avoids any file:// quirks:

```bash
# Python
python -m http.server 8000
# then visit http://localhost:8000

# or Node
npx serve
```

## 🧩 How it's built

- **One file**, plain **HTML + CSS + JavaScript** — no frameworks, no build tooling.
- The logo is embedded as a base64 data URI, so the file is fully standalone.
- The code is organized into commented sections (window manager, file system, each app, themes, assistant, etc.).

## ⌨️ Tips

- `Win` key (or the Start button) opens Start · `Ctrl+Shift+Esc` opens Task Manager · `Alt+R` opens Run
- Right-click the desktop, icons, taskbar, or Start items for context menus
- Control Panel → Recovery → **Reset this PC** restores everything to defaults

## 📦 Notes & limitations

- Horizon has **no real internet access** — it fabricates a page for every address on purpose.
- Browser storage is per-device and per-browser; clearing site data resets the OS.
- The "viruses" are cosmetic simulations contained entirely within the web page.

## 📄 License

MIT — see `LICENSE`. (Add a license file of your choice.)

## 🙌 Credits

Built as a concept project. Icons, apps, and effects are original recreations in the spirit of a desktop OS.
