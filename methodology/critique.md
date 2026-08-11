# The critique

Every batch got these checks plus a read before anything entered the corpus.
The scans are a net under the read, never a substitute for it, and each one
exists because the failure it catches actually happened.

- **Within-dialect near-duplicates.** Jaccard overlap of word 5-gram sets for
  every pair of texts in a dialect, flagged at 0.5, flagged pairs get read.
  Renders of different scenarios should share almost nothing; overlap means
  the writer fell into a rut.
- **Cross-dialect echo.** Same 5-gram Jaccard on renders of the same scenario
  across dialects. Shared bones (the pinned facts) are lawful, shared wording
  is not: wording shared across dialects dilutes exactly the variation this
  corpus exists to carry. Kill bar 0.5; over it, one of the pair gets
  re-rendered after a read.
- **Prompt furniture.** Whole lines wrapped in brackets or parens (the
  stage-direction shape) and literal [placeholder phrase] residue, flagged.
- **Accent talk.** A regex family over "accent", "dialect", "slang", "the way
  we talk", "how they say" and kin. The rule was absolute, the piece is in
  the dialect, never about it. Hits inside a scene still go to the read;
  most are violations.
- **Invented names.** Capitalized tokens mid-sentence, minus sentence starts,
  minus a lawful list (places, brands, institutions, deities, calendar terms,
  variety names). Anything left that recurs is a name candidate, and the cast
  law says roles only.
- **Register tells.** Per-dialect counts of typographic tells, read as rates
  against file counts. The standing one is the em dash: informal speech
  rarely carries it, and a dialect suddenly growing em dashes is drifting
  toward essay register.
- **Band check.** Word counts against the scenario's band. Bands are
  advisory; persistent overrun means restating the ceiling in the prompt,
  never trimming texts by hand.
- **The read.** The scans gate nothing alone. Every batch got a spot read
  regardless, because every new failure mode was found by reading first. A
  condemned text gets replaced by re-rendering its scenario, never edited:
  an edited render stops being a sample of the writer under the
  instructions, and the instructions are what the method controls.
