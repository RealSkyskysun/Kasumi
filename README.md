# Kasumi

A fast, good-looking browser for macOS, in the style of Arc and Zen. Vertical tabs, Spaces, split view and a command bar, built natively in SwiftUI on top of WebKit.

Kasumi is Mac only and needs macOS 14 or later. On macOS 26 and later, Settings and some panels use Liquid Glass.

## Install

1. Download the latest `Kasumi-x.y.z.zip` from the [Releases page](https://github.com/RealSkyskysun/Kasumi/releases).
2. Unzip it and drag `Kasumi.app` into Applications.
3. The first time, right-click the app and choose Open. Kasumi is not notarized by Apple, so macOS asks once.

After that Kasumi updates itself. It checks in the background, or use Kasumi > Check for Updates.

## What it does

**Tabs and Spaces**
- Vertical tab sidebar with pinned tabs, folders, drag to reorder, and a compact mode
- Spaces, each with its own color, icon, cookies and logins, like separate profiles
- Unused tabs are archived automatically, and you can restore them later
- Reopen closed tabs, duplicate tabs, close other tabs, close tabs below, close duplicates, sort by site
- Private tabs that save no history and are gone when you quit

**Split view**
- Two pages side by side or stacked, with a draggable divider
- Drag a tab to the edge of the page to split, swap sides, switch layout, click a pane to focus it

**Command bar**
- One bar for addresses, searches and switching between open tabs, with live suggestions
- Search shortcuts: `yt cats`, `wiki tokyo`, `maps`, `reddit`, `amazon`, `github`, `imdb`, `npm`, `translate`
- Short ones use a bang so they never fire by accident: `!g`, `!ddg`, `!w`, `!gh`, `!so`, `!a`, `!r`, `!m`, `!i`, `!t`

**Reading and pages**
- Find in page, reader view, forced dark pages, mute a tab, page zoom remembered per site
- Save a page as PDF, copy or save a screenshot, view page source, picture in picture
- Copy a clean link without tracking junk, copy a link as Markdown, open the clipboard in a new tab
- Bookmarks, history and downloads in one library

**Privacy**
- Built-in ad and tracker blocker with updatable filter lists, a per-site allowlist and a shield button
- Passkey support
- Search suggestions and history can be turned off
- Import logins, bookmarks and history from Chrome, Brave, Edge, Arc, Vivaldi, Opera, Comet, Firefox, Zen and Safari, or from an exported bookmarks file. Passwords and extensions stay behind

**Extensions**
- Install extensions from the Chrome Web Store and use them from the toolbar
- Kasumi suggests uBlock Origin Lite for network-level ad blocking, including on YouTube
- Support depends on what WebKit allows, so some Chrome extensions will not work

**AI tools**
- Let AI chat sites use this Mac with an approval prompt for each action and an activity log
- An optional remote tool server so Claude and ChatGPT connectors can use Kasumi, with approvals

**Other**
- Cooldown timers for Spaces where you want a break between visits
- Settings built into the window, so it works in full screen
- Colors, theme, animated glass background and tab styling you can change

## Shortcuts

| Key | Action |
|---|---|
| ⌘T | New tab (command bar) |
| ⌘L | Go to address or search tabs |
| ⌥⌘P | New private tab |
| ⌘W / ⇧⌘T | Close / reopen tab |
| ⌘1–9 | Jump to tab |
| ⌃Tab / ⌃⇧Tab | Next / previous tab |
| ⌘S | Toggle sidebar |
| ⇧⌘\ | Toggle split view |
| ⌥⌘S / ⌥⌘L | Swap split panes / stack or side by side |
| ⌃1–9 | Switch Space |
| ⇧⌘N | New Space |
| ⌥⌘N | New folder |
| ⌘[ ⌘] ⌘R | Back, forward, reload or stop |
| ⇧⌘R | Reload from origin |
| ⌘F, ⌘G, ⇧⌘G | Find, next, previous |
| ⌘D | Bookmark this page |
| ⌘Y / ⇧⌘B / ⇧⌘J | History / bookmarks / downloads |
| ⌘= ⌘- ⌘0 | Zoom in, out, actual size |
| ⌥⌘R / ⌥⌘D | Reader view / dark page |
| ⌃⌘M | Mute tab |
| ⌃⌘P | Picture in picture |
| ⌥⌘U | View page source |
| ⌥⌘E | Save page as PDF |
| ⇧⌘C / ⌥⇧⌘C | Copy page URL / copy clean link |
| ⇧⌘V | Open clipboard in new tab |
| ⌘P | Print |
| ⌘, | Settings |
| ⌘-click link | Open in a new tab |

Right-click a tab to pin it, split it or copy its link. Right-click a Space icon to rename, recolor or delete it.

## Not built yet

- Dragging tabs between Spaces
- Pause or resume for downloads
- Full Chrome extension compatibility, which is limited by WebKit

## Build from source

You need macOS 14+ and Xcode 15+ (or the Swift 5.9 toolchain).

- Quick: `swift run` in this folder
- Xcode: open `Package.swift` and press Run
- Check what the importer can see: `.build/debug/Kasumi --check-import`
- Real app: `./build-app.sh` makes `Kasumi.app`, signed with your Apple Development certificate if you have one
- Release: `./release.sh <version> "notes"` builds, zips and publishes to GitHub

Favicons come from Google's favicon service. Swap `Favicon` in `Components.swift` if you would rather not use it.

If you are an AI agent working on this project, read `AGENTS.md` first.
