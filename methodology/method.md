# The method

How I made this, so you could make another one, for more dialects of this
clade or for a different clade entirely. I assume one thing about
linguistics: the dialect is the right resolution to work at.

Two kinds of dialect, two production lines.

## Living dialects

A living dialect gets synthetic texts: a writer (a model under the
instructions in `writer.md`) renders each of 150 fixed scenarios in that
dialect's voice, one text per scenario. The pool is in `scenarios.md` and
the `scenarios/` folder, and the pool is the load-bearing invention:

- **Timeless and regionless.** Scenarios use only perennial human concerns:
  markets, kitchens, roads, weather, work, kin. No brands, no dates, no
  currencies, no pounds or miles, just hours, days, and counts. One pool can
  serve a whole clade.
- **Pinned facts.** Every scenario pins its facts: same events, quantities,
  and cast in every dialect, about one pinned fact per 100 words. What
  varies between renderings is dialect, not plot.
- **Roles, never names.** The cast is the mother, the eldest, the one who
  arrived first. No personal names, pets included. Writers converge on the
  same few invented names, and a shared name counts like a dialect feature.
  It also keeps name-shaped personal data out.
- **Casual register.** Ordinary people speaking plainly. Timeless means
  real, not a theatrical re-enactment.
- **A universality test.** Every scenario must read honest from three lives
  picked far apart. A beat that strains any of them gets replaced.

The pool is regionless, the renderings are not: rupees show up in Mumbai,
because dialects live somewhere and that grounding is signal. Each scenario
also carries an archetype and a length band, defined in `scenarios.md`.

## Dead dialects

A dead dialect gets excerpts, never renderings: real period text only,
sourced in `sources.md`. Captures are cleaned of apparatus, then cut into
contiguous single-source passages: verse on verse lines, prose on sentences
(transcription lines where the edition prints prose that way), one whole
document where the source is a document collection. Same bands and mix.

## If you need a train and eval split

Hold out whole units; units are what leak. For the living the unit is the
scenario: any scenario-level partition is clean, splitting individual texts
is not. For the dead it is the source: excerpts 001 to 100 and 101 to 150
already draw on disjoint sources (whole works, whole documents, or disjoint
regions of one work; `sources.md` maps it exactly).

The ready-made split: the corpus and control marking in `scenarios.md` for
the living, the two excerpt ranges for the dead.

## Quality and curation

Every batch went through the checks in `critique.md` plus a read. The
released texts then got one curation pass. Allowed: deletion, casing,
punctuation. Not allowed: adding anything, dialect markers doubly so; the
one exception is minimal connective tissue already attested in the same
text. Under that law: bracketed stage directions deleted, one clause
discussing accent deleted, a capitalized stress-marker "been" lowercased to
community orthography, and every em dash in the living dialects replaced
with the punctuation it stood for, commas and periods for breaks, ellipses
for cut-off speech (3702 sites; pre-replacement rates varied 20x across
dialects, an essay-register render artifact, not speech; the dead dialects
keep their editions' dashes). Everything else in the writers' voices stands.

## Known characteristics

The warts, so you do not discover them the hard way:

- The writers lean on signature vocabulary far harder than natural text
  would. Measured: 80 near-exclusive markers each appear in at least half of
  their own dialect's 150 files while being absent from nearly all others.
  The worst offenders: b'y in 146 of 150 newfoundland files, enty in 146 of
  gullah, bab in 143 of west-midlands, lah in 141 of singaporean, gert in
  139 of west-country, garans in 130 of anglo-hawaiian, kushti in 129 of
  anglo-traveller, finna in 121 of black-american. The words are real, the
  rates are not, and a classifier trained here can cheat with a small lookup
  table instead of learning structure. Split accordingly, or mask the
  markers if you want to measure anything deeper.
- Bands were advisory; about five percent of texts miss theirs, mostly the
  short band.
- Scenario 50 pins a price of fifteen; the mumbai rendering says 1500. The
  other 25 dialects hold it.
- Beowulfian 001 to 100 draws on five parallel recensions of the Chronicle,
  so word sequences repeat inside that range; 101 to 150 shares none of it.
- The hocclevean documents are one formulary genre; stock openings recur
  across both ranges, though no document appears in both.

## How to propagate the pattern

- A new living dialect: all 150 scenarios rendered, one new directory.
- A new dead dialect: 150 excerpts, the two ranges drawn from disjoint
  sources, plus its entry and map in `sources.md`.
- A new clade: a new directory beside `anglic/`, a roster, a rendering
  campaign. The pool is portable, take it whole.
