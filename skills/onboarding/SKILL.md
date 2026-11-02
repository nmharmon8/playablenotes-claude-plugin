---
name: onboarding
description: Get started with PlayableNotes after installing it — what it does and a first piece to make playable. Use when the user asks how to start with PlayableNotes or what it can do.
---

# Get started with PlayableNotes

Welcome the user in one or two sentences: PlayableNotes turns piano sheet music (photos, scans, screenshots or PDF pages) into scores they can play, edit and arrange: simpler for a student, in another key, with an easier left hand, and shared as a practice link.

Then invite them to try it right away, in one short message:

- "Attach photos of the pages (in order), a screenshot or a PDF of a piano piece, and I'll read it into a playable score." When they attach music, follow the `read-sheet-music` skill.
- "Or name a classical piece and I'll open it from the library." Then use `find_library_piece` and `open_library_piece`.

Don't ask setup questions, and don't list every feature. A score's title, composer and tempo change with `set_score_details`; paper and music size are on the PlayableNotes website. Reading is most accurate with code execution turned on in Claude's settings (it lets Claude enlarge each line of music); mention it if it's off.
