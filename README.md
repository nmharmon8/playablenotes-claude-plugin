# PlayableNotes for Claude

PlayableNotes turns piano sheet music into scores you can play, edit and arrange, right in a conversation with Claude. It is made for piano teachers and their students, church and school musicians, and anyone who plays piano from sheet music.

## What it does

- **Reads sheet music you own.** Send photos, scans, screenshots or a PDF of piano music (a treble and a bass staff), or a MusicXML file, and PlayableNotes reads it note by note into an engraved score.
- **Opens public-domain pieces** from its library: Bach, Mozart, Beethoven, Chopin, Satie, hymns and more.
- **Saves what Claude writes.** Ask Claude for a new piece or exercise, such as "a short waltz in F for a first-year student"; Claude writes the notes and PlayableNotes checks, engraves and saves them.
- **Changes a score on request:** simplify it for a student's level, transpose it, make the left hand easier, fix a wrong note, or check it for reading mistakes. Every change is saved as a new version, so nothing is lost.
- **Shows each score in an interactive card** with playback at any tempo, a measure editor and downloads (PDF, MIDI, MusicXML).
- **Makes practice links** your students can open, play, loop and print without an account.

PlayableNotes works with written music (notation). It does not generate audio, voices or recordings with AI: playback is the notes of the score played on recorded piano samples.

## Use it

In Claude, add the plugin from the plugin directory, or in Claude Code run:

```
/plugin install playablenotes --marketplace nmharmon8/playablenotes-claude-plugin
```

1. Install the plugin, then connect the PlayableNotes connector from the plugin's **Connectors** tab and sign in with your PlayableNotes account (Google or an emailed sign-in link). When connecting you confirm, once, that the music you send is yours or that you may use it for teaching.
2. In a conversation, send sheet music and ask Claude to make it playable, or name a classical piece, or describe a piece you'd like written.
3. Ask for the version you need: "make an easier version for a beginner", "move it to G major", "make a practice link for my student".

The skills in this plugin teach Claude PlayableNotes' score format and how to arrange well for students: `playablenotes` (the tools and the format), `arrange-for-student`, `change-key`, `check-score`, `compose` and `onboarding`.

Your scores live in your PlayableNotes account, the same one as [playablenotes.com](https://playablenotes.com), where you can keep editing on a bigger screen. Reading sheet music uses your account's credits, one per line of music; everything else uses none.

## Data

The plugin contains only instructions (skills) and the address of the PlayableNotes connector, `https://playablenotes.com/mcp`. It runs no code on your computer.

Through the connector, Claude sends PlayableNotes what you ask it to work on: the sheet music you send, the scores Claude writes or changes, titles and settings, and practice-link names. PlayableNotes stores these in your account and reads music with its service providers (Google Cloud and Firebase, and OpenAI for reading pages). It sends nothing else anywhere, and it never receives your Claude conversation beyond what Claude passes to its tools.

You can disconnect Claude, or delete your account and everything in it, on your account page at playablenotes.com. Details: [privacy policy](https://playablenotes.com/privacy), [terms](https://playablenotes.com/terms), [support](https://playablenotes.com/support) (support@playablenotes.com).
