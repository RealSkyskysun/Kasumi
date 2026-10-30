<p align="center">
  <img src="assets/icon.png" width="128" alt="Virga icon">
</p>

<h1 align="center">Virga</h1>

<p align="center">
  A Zen/Arc-style web browser for macOS, built with SwiftUI on the WebKit engine.<br>
  Vertical tabs, Spaces with separate logins, a built-in ad blocker, and more.
</p>

<p align="center">
  <a href="https://github.com/RealSkyskysun/Virga/releases/latest"><b>Download the latest release</b></a>
</p>

---

## Features

**Browsing**
- **Vertical tab sidebar** with pinned tabs, drag-to-reorder, and a compact mode
- **Command bar** (⌘T / ⌘L) to open a URL, search the web with live suggestions, or jump to an open tab
- **Split view** to show two pages side by side
- **Find in page, zoom, print**, and the Web Inspector (right-click → Inspect Element)
- **Bookmarks, history and downloads** in one Library
- **Session restore**: your tabs come back when you reopen the app

**Spaces**
- Each Space is its own profile with **separate cookies and logins**, so you can keep work, school and personal accounts apart
- Pick an icon and a color for every Space; the whole window is tinted to match
- **Cooldown alarm** (optional): set a time like 3:00 PM, hover the Space's icon and start it. The icon shows a ring counting down to that time and a check mark when it's over. It's a reminder only and doesn't block anything.

**Privacy and blocking**
- Built-in **ad and tracker blocker** using community filter lists (EasyList, EasyPrivacy, uBlock Origin, AdGuard, Brave and others), plus YouTube ad blocking
- Pause blocking for a single site with the shield button
- Choose your search engine (Google, Bing or DuckDuckGo) and turn search suggestions and favicons on or off in Settings

**Extras**
- **Passkeys** through Virga's own built-in authenticator
- **Chrome extensions** and the Chrome Web Store, on macOS 15.4 or newer (uses WebKit's web extension support)
- **Import logins from Brave**
- **In-app updates** that check this repo's Releases
- **AI Tools** (optional): lets AI chat sites such as claude.ai and chatgpt.com run a small set of tools on your Mac (read and write files, list folders, run commands). Every call asks for your approval by default. See [A note on AI Tools](#a-note-on-ai-tools).

## Install

1. Download `Virga-<version>.zip` from the [latest release](https://github.com/RealSkyskysun/Virga/releases/latest).
2. Unzip it and drag **Virga.app** into your Applications folder.
3. The first time you open it, macOS may say the app can't be checked for malware, because Virga isn't notarized by Apple. Right-click the app and choose **Open**, then **Open** again. Or go to **System Settings → Privacy & Security** and click **Open Anyway**.

After that, Virga checks for updates by itself (Settings → Updates) and can also be updated from the app menu with **Check for Updates…**.

**Requirements:** macOS 14 (Sonoma) or newer.

## Keyboard shortcuts

| Key | Action |
|---|---|
| ⌘T | New tab (command bar) |
| ⌘L | Go to address / search tabs |
| ⌘W / ⇧⌘T | Close / reopen tab |
| ⌘1–9 | Jump to tab |
| ⌃Tab / ⌃⇧Tab | Next / previous tab |
| ⌘S | Toggle sidebar |
| ⇧⌘\ | Toggle split view |
| ⌃1–9 | Switch Space |
| ⇧⌘N | New Space |
| ⌘[ ⌘] | Back, forward |
| ⌘R / ⇧⌘R | Reload / reload from origin |
| ⌘F, ⌘G / ⇧⌘G | Find in page, next / previous match |
| ⌘= ⌘- ⌘0 | Zoom in, out, reset |
| ⌘D | Bookmark page |
| ⌘Y / ⇧⌘B / ⇧⌘J | History / bookmarks / downloads |
| ⌘P | Print |
| ⇧⌘C | Copy page URL |
| ⌘, | Settings |
| ⌘-click a link | Open in a new tab |

Right-click a tab to pin it, split it, or copy its link. Right-click a Space icon to edit, reorder or delete it.

## Privacy

- Virga has no accounts and no analytics.
- Each Space keeps its cookies and site data separate from the others.
- A few features talk to outside services, and each can be switched off in Settings: search suggestions go to your chosen search engine, favicons come from Google's favicon service, and filter lists are downloaded from their publishers.

## A note on AI Tools

AI Tools is optional and powerful, so treat it carefully. It lets a chat site you choose run commands and read or write files on your Mac. By default Virga shows an approval window for every call, and calls that look risky always ask. An "auto-allow" mode exists but is off by default; only turn it on if you understand the risk. Remote AI Tools, which exposes the same tools to AI services through a private link, always asks for approval unless you separately allow it. Keep that link secret.

## Limitations

- Virga uses the system WebKit engine, not Chromium, so a few sites and extensions behave differently than in Chrome.
- Tabs can't be dragged between Spaces yet.
- Downloads can't be paused or resumed.

## Feedback

Found a bug or have an idea? [Open an issue](https://github.com/RealSkyskysun/Virga/issues).
