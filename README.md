# Rune Clock

Dota 2 rune, camp and objective timers for Windows. It follows the real match
clock through Valve's Game State Integration and calls out bounty, water, power
and wisdom runes, camp pulls and stacks, Roshan, Tormentor and more.

## Download

Grab `RuneClock.exe` from the [latest release](../../releases/latest) and run it.
Nothing to install: Python, Qt and the voice clips are inside the file.

Windows will warn that the file is unsigned — **More info** then **Run anyway**.

## Connect it to Dota 2 (once)

1. In Rune Clock, click **Install config**.
2. In Steam, open Dota 2 → Properties → Launch Options and add
   `-gamestateintegration`.
3. Restart Dota 2. The header turns green and says **LIVE MATCH** when a game
   starts.

Set Dota to **Borderless Window** if you want the overlay drawn on top.

## Updates

Rune Clock can watch this repository and tell you when a new build is out.
In Settings → Updates, switch **Check for updates** on and use this link:

    https://api.github.com/repos/OWNER/REPO/releases/latest

It reads the release info once a day, shows a banner when there's something
newer, and never downloads anything by itself.

This repository holds the downloads only; the source lives elsewhere.
