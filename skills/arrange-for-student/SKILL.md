---
name: arrange-for-student
description: Simplify or adapt a piano score in PlayableNotes for a particular student or level (beginner, early intermediate, an easier left hand, smaller hands, no octaves).
---

# Arranging for a student

The goal is a version this student can play well that still sounds like the piece. Keep the melody recognisable and the harmony intact; remove difficulty, not music.

## First, pin down the student

If the teacher hasn't said, ask one short question, the level or what the student struggles with, unless the request is already specific ("no octaves", "easier left hand"). "A beginner" means level 1. Use the levels below as shared vocabulary. They are a draft based on common method-book sequences (Faber Piano Adventures, Alfred's Basic, RCM / ABRSM grades); the teacher's own description always wins.

| Level | Roughly | Right hand | Left hand | Rhythm | Keys and range |
| --- | --- | --- | --- | --- | --- |
| **1 · First year** | Primer to Level 1; pre-Grade 1 | Melody only, mostly steps and skips within a five-finger position; one position shift at a phrase | Single notes or open fifths, one per measure or per half note | Whole, half, quarter; dotted half; quarter rests | C, G, F major and A minor; within two octaves of middle C; no ledger lines past two |
| **2 · Late beginner** | Level 2 to 3A; Grade 1 | Melody with occasional two-note intervals; small shifts | Root-position triads or root and fifth on strong beats; simple broken chords in quarters | Adds eighth pairs, dotted quarter and eighth, ties | Up to two sharps or flats |
| **3 · Early intermediate** | Level 3B to 4; Grades 2 and 3 | Melody with thirds and sixths and simple ornaments written out | Alberti or broken-chord patterns in eighths; inversions; occasional bass line | Sixteenths in short groups, syncopation, triplets | Up to three sharps or flats; hand-crossing rare |
| **4 · Intermediate** | Level 5 and beyond; Grades 4 and 5 | Close to the original; thin only the thickest textures | Most patterns kept; octaves allowed | Original | Original key unless asked |

## Techniques (lightest first)

1. **Thin chords**: keep the melody (top) and the bass (bottom), and drop inner doublings. Keep the third of the chord when you can, because it defines the harmony.
2. **Simplify the accompaniment**: turn running patterns into block chords on the beat. For example, an Alberti bass in eighths becomes one chord per half measure, then one chord per measure.
3. **Remove octaves**: keep the note in the most comfortable register, usually the upper note in the left hand and the lower in the right.
4. **Simplify rhythm**: turn dotted figures into even values, sixteenth runs into eighths, and fast ornaments into the main note, while keeping the melody's shape.
5. **Narrow the range**: move passages by an octave to stay near the middle of the keyboard. Move whole phrases, not single notes.
6. **Shorten runs and arpeggios**: keep the start and the target note, and cut the middle.
7. **Change the key** (only if the teacher allows it): to one with fewer accidentals. See `change-key`.

At levels 1 and 2 the level comes first: a first-year version has no sixteenth-note runs, and a piece much longer than about 32 measures is arranged as its main theme (for Für Elise, the A section with its repeat); say which measures you kept. Where its notes are too fast (sixteenths in 3/8), double every value and the beat with it: 3/8 becomes 3/4, one measure stays one, and every note of the tune stays. Pass a tempo with the edit (twice the old number keeps the original speed; for a beginner choose slower, about 100 for Für Elise), and say the time signature changed. If eighth notes remain, call it "a late-beginner version" and offer a plainer one in quarter notes; don't rewrite the melody unless the teacher takes that offer.

Otherwise keep the meter, the number of measures, repeats, dynamics, slurs and articulations. If a measure can't be simplified without losing the tune, simplify the left hand more and the right hand less.

## Doing it in PlayableNotes

1. Call `get_score` (it includes KM in brief) and look at the whole piece first: the melody and the harmony in each measure. If what was asked for is already true, say so and offer the next step down instead of saving a change that isn't one.
2. Decide on one consistent treatment for each section. For example, "LH: one chord per measure, root position; RH: melody only, no octaves".
3. For a whole-piece arrangement, send the whole KM to `edit_score`. Every voice line must still add up to the measure, and `s/` spacers must stay where voices drop out.
4. Check both hands against the level's row before saving, and say only what the notes show: the level reached and what stays hard.
