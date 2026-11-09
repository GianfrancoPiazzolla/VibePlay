<div align="center">

# 🎧 VibePlay 🎶

**A local-first music player for the browser — local files, whole folders, live streams and audiobooks in one queue.** 🎧🚀

[![Made with HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](#-tech-stack)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](#-tech-stack)
[![Vanilla JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](#-tech-stack)
[![No build step](https://img.shields.io/badge/No_build_step-0b0d11?style=for-the-badge&logo=checkmarx&logoColor=22d3ee)](#-tech-stack)
[![Local-first](https://img.shields.io/badge/Local--first-100%25-22d3ee?style=for-the-badge&logo=shield&logoColor=white)](#-privacy--data)
[![License MIT](https://img.shields.io/badge/License-MIT-34d399?style=for-the-badge&logo=opensourceinitiative&logoColor=white)](#-license)

[https://vibeplay-one.vercel.app/](https://vibeplay-one.vercel.app/)

</div>

---

## 📚 Table of Contents

- [🌟 What is VibePlay?](#-what-is-vibeplay)
- [🎧 Built for Audiobook Listeners](#-built-for-audiobook-listeners)
- [✨ Features](#-features)
- [🎚️ The Player](#-the-player)
- [🎵 Supported Sources](#-supported-sources)
- [🚀 Quick Start](#-quick-start)
  - [🎬 First steps](#-first-steps)
- [⌨️ Keyboard Shortcuts](#-keyboard-shortcuts)
- [🔐 Privacy & Data](#-privacy--data)
- [📦 Backup & Restore](#-backup--restore)
- [🧠 Tech Stack](#-tech-stack)
- [🗂️ Project Structure](#-project-structure)
- [🌍 Browser Support](#-browser-support)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)

---

## 🌟 What is VibePlay?

VibePlay is a **single-page music player** that runs entirely in your browser. Load a local audio file, a whole folder, or a direct stream URL, give each one a **reference name**, and it becomes a reusable *source* in your personal library. Build a queue, reorder it by drag & drop, skip what you don't want, and keep listening with shuffle, repeat, bookmarks, resume points, a sleep timer and variable playback speed.

> 🎧 **Audiobook-first by design.** Long narrations, books split into dozens of files, chapters to revisit and sessions that end with you falling asleep — those are the needs VibePlay was built around.

> 🛡️ **Nothing is uploaded.** Audio never leaves your device: the app only stores source metadata, settings, bookmarks and resume positions inside your browser.

---

## 🎧 Built for Audiobook Listeners

VibePlay is not a generic player with audiobook support bolted on: **its features were created specifically to meet the needs of people who love listening to audiobooks** 🎧📚. Every control on screen answers a real listening problem — from losing your place in a 12-hour novel to rewinding the last sentence you half-heard.

| 🎧 Audiobook need | ✅ How VibePlay answers it |
|---|---|
| ⏳ **Never lose your place** | Resume points are stored per track and offered again when you reopen a local file or folder book. |
| 🔖 **Mark chapters, quotes and notes** | Named bookmarks per track, listed in a dedicated panel and drawn on the seekbar with tooltips. |
| 📚 **Books split into many files** | Drop the whole book folder 📁: tracks are scanned recursively, sorted by name and advanced automatically. |
| 🚫 **Skip intros, credits and samples** | Exclude any source from the playlist with one click 👁️‍🗨️ while keeping it in the library. |
| 🎚️ **Slow or fast narrators** | Playback speed from **0.10× to 10×**, saved for the next session. |
| ⏲️ **Fall asleep while listening** | Sleep timer from 1 to 720 minutes with a live countdown pill, working even while paused. |
| ⏪ **Re-listen to the last sentence** | Dedicated −30 s / +30 s buttons, plus 5 s and 30 s arrow-key seeks. |
| 🏷️ **Book and author metadata** | ID3v2 / ID3v1 parsing for title, artist and album — album often carries the book title. |
| 🔍 **Large libraries** | Reference names, instant filtering and drag & drop queue ordering keep hundreds of books manageable. |
| 💾 **Move your library** | JSON backup and restore with merge or overwrite, so bookmarks and resume points travel with you. |
| 📴 **Listen offline** | A service worker caches the app shell, and every local file stays on your device. |

> 🎯 In short: music players optimize for three-minute songs. **VibePlay optimizes for chapters, hours and the bookmark you left at 2 a.m.** 🌙🔖

---

## ✨ Features

| | Feature | Description |
|---|---|---|
| 🎧 | **Audiobook-first** | Bookmarks, resume points, variable speed, sleep timer and folder books built for long-form listening. |
| 📂 | **Local files & folders** | Pick an audio file, or drop files and whole folders anywhere on the page. |
| 🌐 | **Direct streams & HLS** | Play direct audio URLs and `.m3u8` HLS streams (native on Safari, via `hls.js` elsewhere). |
| 🏷️ | **Named sources** | Save each source under a reference name; rename it any time with the ✏️ button. |
| 🧭 | **Queue control** | Move sources ⬆️⬇️, drag rows to reorder, filter with the 🔍 search box. |
| 🚫 | **Exclude from playlist** | Keep a source in the library but skip it in the queue with the 👁️‍🗨️ toggle. |
| 🔀 | **Shuffle & repeat** | Shuffle across included sources; repeat off 🔁 / all 🔁 / one 1️⃣. |
| 💾 | **Session-only sources** | Turn saving off to listen now without storing the source (🟡 TEMP badge). |
| 🔗 | **Relink files** | Reconnect a saved local source to its file with one click when the browser forgets it. |
| ↩️ | **Undo remove** | Removing a source shows a toast with an **UNDO** action. |
| 🎚️ | **Playback speed** | Fine-grained range from **0.10× to 10×**, saved between sessions. |
| ⏲️ | **Sleep timer** | Stop playback after 1–720 minutes, with a live countdown pill. |
| 🔖 | **Bookmarks** | Named markers per track, shown on the seekbar and in a dedicated list. |
| ⏯️ | **Resume points** | Every local track remembers where you stopped and offers to resume. |
| 📊 | **Waveform & spectrum** | Decoded waveform for local tracks and a live spectrum analyzer for playing audio. |
| 🎛️ | **Seekbar intelligence** | Hover markers for bookmarks and resume points, plus ±30 s jump buttons. |
| 🖥️ | **Media Session** | Track metadata and OS media keys where supported. |
| 📦 | **Backup & restore** | Export/import the whole library as JSON, with **merge** or **overwrite**. |
| 🌙 | **Polished dark UI** | Responsive layout, vinyl disc animation, toasts, reduced-motion support. |
| 📴 | **Service worker** | Caches the app shell for offline use (see the icon note below). |

---

## 🎚️ The Player

```
💿 spinning disc  →  play / pause on click
🖼️  cover initials →  generated colour gradient per source name
📈  waveform       →  local tracks · 🌈 live spectrum  →  analysers
🎯  seekbar        →  bookmarks 🔖 and resume points 🟢 markers
⏱️  times          →  current · ±30 s · duration / LIVE
🔊  volume         →  slider + mute
⏲️  sleep timer    →  countdown pill with quick cancel
🔁  transport      →  shuffle · previous · play · next · repeat
```

---

## 🎵 Supported Sources

| Icon | Type | Details |
|---|---|---|
| 💻 | **Local file** | Single audio file from your device, kept in IndexedDB for one-click access. |
| 📁 | **Folder** | Drop a folder for a recursive scan; every audio file becomes a track, sorted by name. |
| 🎧 | **Audio URL** | Direct links to `.mp3`, `.m4a`, `.aac`, `.ogg`, `.oga`, `.opus`, `.wav`, `.flac`, `.webm`, `.aif`, `.aiff`. |
| 📡 | **HLS stream** | `.m3u8` playlists, with native support on Safari and `hls.js` on other browsers. |

---

## 🚀 Quick Start

```bash
# 📥 1. Clone the repository
git clone https://github.com/GianfrancoPiazzolla/VibePlay.git
cd VibePlay

# 🌐 2. Serve the folder with any static server
python -m http.server 8080

# ▶️ 3. Open the player
#    http://localhost:8080
```

> 💡 You can also open `index.html` directly, but a local server is recommended so the service worker and File System Access API behave consistently.

### 🎬 First steps

1. ➕ Click **+** (or drop an audio file / folder on the page).
2. 🏷️ Type a reference name, choose **LOCAL FILE** or **STREAM URL**.
3. 💾 Keep **Save to my sources** on for later, or turn it off for a 🟡 TEMP source.
4. ▶️ Hit **PLAY**, then drag rows to order your queue. 🎉

---

## ⌨️ Keyboard Shortcuts

| Key | Action |
|---|---|
| <kbd>Space</kbd> | ▶️⏸️ Play / pause |
| <kbd>←</kbd> / <kbd>→</kbd> | ⏪⏩ Seek 5 seconds |
| <kbd>Shift</kbd> + <kbd>←</kbd> / <kbd>→</kbd> | ⏪⏩ Seek 30 seconds |
| <kbd>N</kbd> | ⏭️ Next track |
| <kbd>P</kbd> | ⏮️ Previous track |
| <kbd>M</kbd> | 🔇 Mute / unmute |
| <kbd>B</kbd> | 🔖 Open bookmarks |
| <kbd>Enter</kbd> / <kbd>Space</kbd> on a row | ▶️ Play that source |
| <kbd>Esc</kbd> | ❌ Close the open dialog |

---

## 🔐 Privacy & Data

VibePlay is **100 % client-side** 🛡️ — no accounts, no analytics, no server, no uploads.

| Icon | Stored data | Where |
|---|---|---|
| 🗂️ | Sources library (names, types, URLs, durations, metadata) | `localStorage` → `vibeplay.sources.v1` |
| ⚙️ | Settings (volume, shuffle, repeat, speed, last source) | `localStorage` → `vibeplay.settings.v1` |
| 🔖 | Bookmarks | `localStorage` → `vibeplay.bookmarks.v1` |
| ⏱️ | Resume points | `localStorage` → `vibeplay.resume.v1` |
| 📎 | Local file/folder handles | IndexedDB → `vibeplay` / `handles` |

> 🧹 Clearing site data resets the library. Local sources may then need a new file picker selection via **RELINK** 🔗.
> 🟡 **TEMP** sources are intentionally never persisted.

---

## 📦 Backup & Restore

Open **DATA** 🗄️ in the header to:

- 📤 **Export backup** — a JSON file with sources, settings, bookmarks and resume points.
- 📥 **Import backup** — preview a summary, then choose:
  - 🧩 **MERGE** — add new sources and bookmarks, keep your current settings.
  - ♻️ **OVERWRITE** — replace everything, including volume and speed.

```json
{
  "app": "VibePlay",
  "version": 1,
  "exportedAt": "2026-01-01T00:00:00.000Z",
  "settings": { "volume": 0.8, "shuffle": false, "repeat": "off", "rate": 1 },
  "sources": [{ "id": "…", "name": "Late night set", "kind": "url", "url": "https://…" }],
  "bookmarks": { "url:…": [{ "id": "…", "time": 42.5, "name": "Chapter 2" }] },
  "resumePoints": { "local:…": 128.4 }
}
```

> 🎵 Audio files are **not** included in backups: local files and folders must be relinked on the new device.

---

## 🧠 Tech Stack

| Icon | Technology |
|---|---|
| 🧱 | **HTML5 + CSS3 + vanilla JavaScript** — one self-contained `index.html`. |
| 🎧 | **HTMLAudioElement** for playback and **Media Session API** for OS integration. |
| 🌈 | **Web Audio API** — analyser node for the spectrum, `decodeAudioData` for the waveform. |
| 🗃️ | **IndexedDB** for file/folder handles, **localStorage** for the library. |
| 📡 | **hls.js** loaded on demand from jsDelivr for non-Safari HLS playback. |
| 🧾 | **ID3v2 / ID3v1** tag parsing for title, artist and album. |
| ⚙️ | **No frameworks, no bundler, no dependencies to install** 🎉 |

---

## 🗂️ Project Structure

```
📦 VibePlay
├── 🌐 index.html   # app shell — markup, styles and all player logic
├── 🖼️ favicon.ico  # site icon
└── 📴 sw.js        # service worker — caches the app shell for offline use
```

> 🧩 `sw.js` lists `icon-192x192.png` and `icon-512x512.png` in its cache manifest: add those two files (or remove them from the list) so the service worker installs cleanly and offline caching works.

---

## 🌍 Browser Support

| Browser | Status |
|---|---|
| 🟢 Chrome / Edge (Chromium) | ✅ Recommended — including folder access and handle persistence |
| 🟢 Safari | ✅ Works — native HLS playback |
| 🟡 Firefox | ✅ Single files and streams; dropped folders and saved handles are limited |
| 📱 Mobile browsers | ✅ Responsive UI; file picker instead of folder access |

> 🎨 Visualizer and waveform need **Web Audio API** support. Cross-origin streams must allow CORS for analysis.

---

## 🤝 Contributing

Contributions, ideas and bug reports are welcome! 🎉

1. 🍴 Fork the repository.
2. 🌿 Create a branch: `git checkout -b feat/my-idea`.
3. ✏️ Make your changes and test them in the browser.
4. 📬 Open a pull request with a clear description.

Found a bug? 🐞 Open an issue with steps to reproduce and your browser version.

---

## 📜 License

Distributed under the **MIT License**. Feel free to use, modify, and share.

---

> 🌱 *Made with ❤️ and 🧠. If you find this tool helpful, please leave a ⭐ on GitHub!*