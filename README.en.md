# Cartridge — Tester Guide

*[Leer en español](README.md)*

Thanks for helping out with this project! Cartridge is a native macOS
launcher for Pokémon fangames made with RPG Maker XP / Essentials. The
idea is simple: hit PLAY and the game just runs — no Wine, no manual
setup.

This is an **experimental, actively developed** project, so your testing
is genuinely valuable for finding things we haven't covered yet.

## Download

👉 **[Grab the latest version here](https://github.com/United2204/cartridge-releases/releases/latest)**
(the `Cartridge.zip` file). That's all you need — once installed, the app
updates itself (see below).

## Requirements

- macOS (Apple Silicon or Intel — the app is universal, runs natively on
  both).
- Your games already unzipped into a folder (or the original `.zip`/`.rar`
  files, which you can unzip yourself with Finder / Archive Utility).
  **Important: that folder can NOT be inside Downloads** — move it to
  Documents, Desktop, or any other location before selecting it in
  Cartridge.

## Installation

Cartridge is now signed and notarized by Apple, so it installs like any
other app:

1. Unzip the `.zip` you downloaded and move `Cartridge.app` to your
   Applications folder (or wherever you prefer).
2. **Double-click to open it.** You shouldn't see any security warning.
   - If you do get a Gatekeeper warning anyway (for example if you
     downloaded an old unsigned build), click **Open** anyway, or go to
     **System Settings → Privacy & Security** and confirm from there.

## Automatic updates

Since **beta 4**, Cartridge **updates itself**. When we publish a new
version, the app offers it to you on launch and installs it with one
click — you don't have to download anything by hand or repeat the steps
above.

To check manually at any time, use the **Cartridge → "Check for
Updates…"** menu (top-left, in the menu bar).

> If you were on an old beta (1, 2 or 3) that's no longer in the list,
> those didn't have auto-update: download the latest from the link above
> and it'll keep itself up to date from then on.

## How to use it

1. The first time you open it, it'll ask you to pick the folder where you
   have (or will have) your unzipped games. It remembers this for next
   time.
2. Detected games show up in a grid with their cover art. Some need a
   one-time compatibility conversion (you'll see a small "APPLYING
   PATCH…" progress bar) — that's automatic, nothing to do on your end.
3. Hit PLAY and you're in.

## What to test

The most useful thing you can do is just play like you normally would:
progress through the story, get into battles (wild and trainer), save and
load your game, move between maps/routes, and if the game supports it,
evolve Pokémon, use items, open menus, etc. The further you get, the
better — most of the issues found so far only show up in specific
situations (a particular route, a particular animation), not on startup.

## Known limitations (for now)

- **Online features that use direct LAN-style connections** (for example,
  some Cable Club variants over local network) aren't supported yet.
  Online features that use regular HTTP/HTTPS (checking for updates,
  GTS-style trades, etc.) should work fine.
- It's possible some specific game with very unusual scripts won't boot or
  will fail at a specific point — if that happens to you, that's exactly
  the kind of thing we want you to report.

## How to report a problem

If something breaks, send us:

1. **Which game** (name, and version if you know it).
2. **What you were doing** right before it happened (e.g. "entered a wild
   battle on Route 3", "loaded a saved game").
3. **A screenshot** of the error, if one appeared.
4. If you can reproduce it more than once, tell us the steps — that helps
   the most.

It doesn't need to be a formal report — a message describing what you saw
is enough.

We also have a Discord for bug reports, chat, and news:
**<https://discord.gg/XjurW8XXPf>**

## Support the project

Cartridge is a personal project, built in spare time. If you like it and
want to support development, you can buy me a coffee here:
**<https://ko-fi.com/united2204>** — totally optional, doesn't affect the
app or this beta in any way.

Thanks again for testing it!
