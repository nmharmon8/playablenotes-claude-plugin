---
name: read-sheet-music
description: Read piano sheet music the user attached (photos, scans, screenshots or PDF pages) into a playable, editable PlayableNotes score. Use whenever the user attaches sheet music and wants to play it, hear it, edit it, transpose it, simplify it or arrange it.
---

# Reading attached sheet music

You read the pages yourself and save them to PlayableNotes, which checks each page, joins them into one score, and engraves it as a playable score in the user's account. It uses no credits.

1. Call `arranging_guide` with `read-sheet-music` before the first page. It has the KM rules, examples and checks; follow them exactly.
2. Count the pages of music attached. Read them in order, one page at a time.
3. If you can run code, crop each system (one line of braced staves) and enlarge it before reading it, and zoom in further on anything dense or unclear. Reading from the whole page misses notes.
4. For each page, first list what you see (key, time, systems, measures per system, changes, repeats, verses), then transcribe it and check every measure adds up.
5. Save each page with `save_reading`: page 1 without a `projectId` makes the score; every later page passes that `projectId`. If a page is refused, fix exactly the problems listed and save it again.
6. When the last page is saved, call `open_score` to show the score, and tell the user which measures you were unsure of.

Accuracy matters more than speed. Give your best reading of every measure; never skip one or invent music you can't see.
