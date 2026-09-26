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

From 1.6.0, Rune Clock keeps itself up to date. Each time it opens (and every
few hours while it runs) it looks at the latest release here, downloads the new
`RuneClock.exe`, checks it against the SHA-256 published with the release, and
restarts into it. It never restarts during a match; a download that arrives
mid-game waits until the match is over.

You can turn this off in Settings → Updates and get a banner with a Download
button instead. Copies older than 1.6.0 can't update themselves, so download
1.6.0 once by hand.

## Builds tab

From 1.8.0 the **Builds** tab shows, for any hero and position: starting items,
the most common skill order for levels 1–10, talent pick and win rates, and
core items with the minute they're usually finished. The numbers come from
[STRATZ](https://stratz.com) (Legend rank and above, this week) and the icons
from Valve. It switches to the hero you're playing when a match starts.

The app downloads the data from the **Hero builds data** release here twice a
day. That release is data, not an app version, so it never counts as an update.

This repository holds the downloads only; the source lives elsewhere.
