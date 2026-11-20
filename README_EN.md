[English](README_EN.md) | [Русский](README.md)

<div align="center">
  <h1>AINotes</h1>
  <p>
    <i>One exe, endless possibilities.</i>
  </p>
</div>

**AINotes** is a lightweight background utility for Windows (10, 11) that lives in your system tray and turns any selected text, code snippet, file, or folder into an instant knowledge base with one-click pasting right at your cursor.

> This is not a bloated note-taking suite. The core idea is to capture a code snippet, terminal command, or project folder path in a single click, and paste or launch it anywhere in a fraction of a second.

---

## Network Hygiene & Privacy

The utility is built on the principle of **Zero Network Footprint**:
* **No network access:** the executable contains no networking modules, never connects to external servers, and performs no background update checks.
* **Zero telemetry:** no user data, keystrokes, or clipboard contents are ever collected, analyzed, or transmitted.
* **100% local storage:** your SQLite database (`notes.db`), settings (`config.json`), and localization files stay strictly on your local drives.

---

## Key Features

* **Instant Capture for Text, Files & Folders**
  * **For text & code:** highlight any fragment with your mouse — it is automatically copied to the clipboard (ready for immediate `Ctrl + V`) while a pulsing beacon appears near the cursor. Click it to save the item into a group and assign a priority from 1 to 5 stars.
  * **For files & folders (fast project navigation):** select a file or folder in Windows Explorer and gently drag it to the right (holding Left Click without `Ctrl` or `Shift`) — the save beacon will appear. Supports batch selection and any special characters in names (`[ ]`, spaces, Unicode).
* **Organized Groups with Accordion View**
  Groups are displayed as a collapsible accordion with item counters: text snippets with star ratings appear at the top, followed by a clean list of saved folders and files with quick buttons to open in Windows, copy the path, or delete.
* **Smart Sorting & Duplicate Protection**
  * Item order is calculated using combined weight: **priority (stars) + usage frequency**. Your most needed snippets stay right at the top.
  * Saving identical text never creates duplicates — instead, the usage counter increases and the star rating automatically upgrades to the higher value.
* **Paste at Cursor & Flexible Shortcuts**
  Press your shortcut (default `Alt + V` or a custom combo like `Shift + Left Click` / `Ctrl + Left Click`), filter via live search, and paste directly into the active text cursor. Key detection is bound to hardware scan codes and works reliably regardless of your active keyboard layout.
* **Long Notes & Inline Editing**
  Click any group title or note line to edit it directly in place. Multi-line snippets can be expanded inside the card to copy specific lines and collapsed back into a single row.
* **Window Memory & Multi-Monitor Support**
  Every dialog opens centered on the active monitor (where your cursor is located) on first launch, and remembers its custom position and size in `config.json` thereafter.
* **Automatic Backup & Dated Export**
  Whenever changes occur, `notes.db` is silently mirrored to your designated backup folder (e.g., on a secondary drive). Exporting all notes to a text file (`all_notes_YYYY_MM_DD_HH-MM.txt` in UTF-8 grouped cleanly by category) also saves a copy to the backup folder.
* **Multi-Language Support (`RU` / `EN` / `ZH` + Custom Locales)**
  Interface translations are stored in external `.ini` files inside the `locales/` folder. You can open the folder from the tray menu at any time to add your own language file.

---

## Installation & Quick Start

1. [Download](https://github.com/EuSPb24/AINotes/releases/download/notes/AINotes_Setup_1.3.0.exe) **`AINotes_Setup_1.3.0.exe`** (direct download) or pick a release on the [Releases](https://github.com/EuSPb24/AINotes/releases) page.
2. Run the installer (no additional runtime or Python installation required). During setup, choose your primary folder for the notes database and an optional backup folder on another drive.
3. The utility icon will appear in your Windows system tray: green **N** = capture active, red **N** = paused (left-click the tray icon to toggle).

---

## Controls & Shortcuts

| Action | Control |
| :--- | :--- |
| Capture text / code | Highlight with Left Click (auto-copies to clipboard + shows beacon) |
| Capture file or folder | Select in Explorer and gently drag right with Left Click (without `Ctrl`/`Shift`) |
| Open paste & search menu | `Alt + V` (default) or custom shortcut from settings (e.g. `Shift + Left Click`) |
| Toggle capture ON / OFF | Left-click the **N** icon in the system tray |
| Edit group or note inline | Click the text inside any card, edit, and press `Enter` (or click away) |

---

Distributed free of charge under the [Freeware License].

## Authors

**AINotes** was created in live symbiosis by **EvGen** and **Gemini AI Assistant (Google)**.  
2026 | `v.1.3.0`

<div align="center">
  <br/>
  <img src="logo.png" alt="AINotes Symbiosis Logo" width="110" height="110" />
</div>
