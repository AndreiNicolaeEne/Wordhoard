# The writer instructions

Every synthetic text came from a writer: a Claude Sonnet 5 given one
assembled prompt and nothing else, fresh session per text, no memory of any
other rendering. The renders ran through the second and third quarters of
2026. This file is the prompt's anatomy, verbatim where the wording is the
point.

## The prompt, assembled per dialect and scenario

Six parts, in order.

**1. Persona.** One line: "You live in <city>." The dialect's home place,
place and person, never a dialect name. Inhabit, not perform: name the
dialect and you get its stereotype, name the place and you get its people.

**2. Frame.** Verbatim:

> You are an ordinary person there, and so is everyone in what follows. Write
> the piece below from inside that life: if it is you speaking or writing, it
> is in your own everyday voice; if it is an exchange between other people,
> they are people around you, and it goes down the way such people would
> really say it.

**3. Purpose.** Verbatim, and it earns its keep: renders without it hedge
toward standard register, renders with it commit. This is the wording the
writers got during production; it describes the campaign that commissioned
the texts, not this corpus, which has no mission beyond providing data.

> Why this matters: automated language-ID and quality filters misclassify and
> delete minority-dialect text at scale; measured on real pipelines, most of
> it never survives into datasets or models. That is erasure of real people's
> speech from the record. This project builds a classifier that can recognize
> these varieties so pipelines stop destroying them. Faithful, fully textured
> dialect writing is the point of this task, not a risk in it: write the
> speech the way it is actually spoken and written, spelling, grammar, rhythm
> and all. What stays out of bounds is the same as ever: no talking ABOUT the
> accent inside the piece, no tourist color, no quaintness. The people are
> ordinary people; their speech is theirs.

**4. The scenario.** The record's `text` field, verbatim. The only part that
changes between scenarios.

**5. The brief.** A short advisory note on the dialect, introduced verbatim
as:

> A linguist's notes on the speech of your place, advisory. Use what fits
> naturally, never force it; grammar and rhythm carry more truth than slang:

followed by an itemized list of what the dialect looks like on the page.
Written once per dialect and kept advisory: a forced shibboleth is worse
than none.

**6. Rules.** Stated plainly at the end:

- The length aim for the scenario's band (about 30 to 80, 150 to 400, or 800
  to 2000 words); short-band prompts add "stay under 80".
- Never talk about the accent, dialect, or word choices inside the piece;
  full texture wanted, spelling, grammar, rhythm and all.
- Dialogue is speaker-labeled turns, and the labels are role words.
- Everyone is called by role, relation, or address word, never an invented
  personal name, animals included.
- No dates, no addresses, no headers.
- Write only the piece.

## Per-dialect additions

- Dialects that weave English with another language get one added line:
  "Keep the piece in <dialect> English, <other language> woven in where
  natural." Without it, writers either purge the other language or fall into
  it wholesale, and the weave is the interesting register.
- Where a dialect spans a register continuum, the target register was ruled
  once and stated in the prompt from then on.
- Every dialect renders under its own brief, the anchor included. An anchor
  rendered without a brief would measure the model's habits, not the dialect.

## Mechanics

- One fresh writer per text, no shared context. Convergence is the enemy of
  a corpus that is supposed to vary.
- Prompts generated to files first; a writer reads its one prompt and writes
  its one output.
- One retry on mechanical failure only (an empty file, a refusal), never on
  quality; quality goes to the critique.
- Refusals were preserved and counted per batch as a health signal on the
  instructions; none ship with the corpus.
