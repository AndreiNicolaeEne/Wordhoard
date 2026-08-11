# The scenario pool

The 150 scenarios behind every synthetic text, verbatim, split by category
into the files under `scenarios/`. A scenario's number is its filename number
everywhere: `scenario-017.txt` in any dialect directory is that dialect's
take on scenario 17.

| category | scenarios | total | corpus | control |
| --- | --- | --- | --- | --- |
| birth | 1 to 5 | 5 | 3 | 2 |
| childhood | 6 to 13 | 8 | 5 | 3 |
| love | 14 to 22 | 9 | 6 | 3 |
| marriage | 23 to 29 | 7 | 5 | 2 |
| food | 30 to 37 | 8 | 6 | 2 |
| work | 38 to 45 | 8 | 5 | 3 |
| trade | 46 to 53 | 8 | 5 | 3 |
| house | 54 to 61 | 8 | 6 | 2 |
| neighbors | 62 to 71 | 10 | 7 | 3 |
| friends | 72 to 80 | 9 | 6 | 3 |
| body | 81 to 89 | 9 | 6 | 3 |
| death | 90 to 97 | 8 | 5 | 3 |
| memory | 98 to 102 | 5 | 3 | 2 |
| journeys | 103 to 112 | 10 | 7 | 3 |
| games | 113 to 120 | 8 | 5 | 3 |
| night | 121 to 126 | 6 | 3 | 3 |
| weather | 127 to 134 | 8 | 5 | 3 |
| anger | 135 to 143 | 9 | 7 | 2 |
| verse | 144 to 150 | 7 | 5 | 2 |

The corpus and control columns mark the split described in `method.md`; the
marking is frozen.

## Reading a record

```
=== scenario 1 | birth | M | m | corpus ===
scenario: <the one-line idea the record grew from>
zones: <expected features, audit tags only; the text never names them>
intent: <one sentence: what the piece is>
beats: <the events of the piece, in order>
held: <the pinned facts: same in every dialect's rendering>
cast: <roles and relations only, never names>
text: <the paragraph handed to the writer, verbatim>
=== end ===
```

Header order: number, category, archetype, band, side of the marking.
Archetypes: M is one voice addressed to "you" and the addressee never speaks,
D is an exchange, V is verse, P is a posted notice. Bands: s 30 to 80 words,
m 150 to 400, l 800 to 2000, mixed at roughly 3:4:3.

Only the `text` field ever reached a writer (see `writer.md`). The rest is
authoring scaffolding: the beats plot the piece, the held list pins the facts
that must survive into every dialect, and the zones name what the scenario is
expected to exercise, so coverage across the pool could be audited.
