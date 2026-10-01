# NOVA CORTEX — INFORMATION CORPUS

Publication and knowledge layer derived from NOVA CORTEX LAB.

**Status:** working document, not canonical.
Conceptual direction: see `meta/context.md` in the parent
repository (LAB). Corpus-specific scope below.

---

## Purpose

The Corpus makes the development of NOVA CORTEX LAB research
understandable, traceable, and accessible at different depths:
to a casual reader, to a technical reader, to a researcher,
to another AI system, and to the project author.

It is not a replacement for LAB. LAB is the primary research
environment. The Corpus is derived from it and never becomes
the authoritative source merely because it is easier to read.

## Relationship to LAB

    NOVA CORTEX LAB  ->  DDA  ->  CORPUS  ->  publications

LAB contains experiments, traces, methodology, results,
branch history, unresolved questions. The Corpus transforms
selected LAB material into accessible, connected research
objects.

Primary references must remain traceable to LAB.

## Structure

    corpus/
    ├── ru/   ← working layer (Russian)
    └── en/   ← publication / discovery layer (English)

Russian is the author's working language.
English is the primary external and machine-readable language.

The two versions are linked representations of the same
object, not two independent systems. Each file links to its
counterpart in the other language.

## Layers (depth)

- **Layer 0 — POINT.** Short object, ~2–3 minutes.
  One primary thing: observation, experiment, result,
  conceptual distinction, methodological change, open problem.
- **Layer 1 — SEQUENCE.** Related POINTs form a local
  trajectory: question → experiment → result → correction →
  next question.
- **Layer 2 — DEEP.** Substantial material: hypotheses,
  reasoning, ontology, competing interpretations,
  methodological failures, unresolved contradictions.
- **Layer 3 — PRIMARY CORPUS.** Direct links to LAB source:
  experiments, traces, METHOD, CONCEPT.
- **Layer 4 — PARTICIPATION.** Optional: read → inspect →
  verify → reproduce → extend.

Current stage: POINT objects only.

## Status vocabulary

Every corpus object carries an explicit status
(per Information Corpus §9):

- `FACT` — confirmed, traceable to a primary source.
- `RESULT` — outcome of a completed run or experiment.
- `INTERPRETATION` — author's analysis, not a fact.
- `HYPOTHESIS` — an assumption, not yet tested.
- `OPEN` — unresolved question.
- `HISTORICAL` — superseded or past state.

A publication must not silently convert:

- interpretation into fact,
- hypothesis into result,
- experimental observation into general claim,
- historical state into current methodology.

When evidence is insufficient, uncertainty is preserved.

## Adding new POINT objects

1. Choose a distinct, useful research object from LAB.
   Not every artifact deserves publication.
2. Write `ru/` first — the working version.
3. Mirror into `en/` — the publication version.
4. Carry an explicit status.
5. Link to primary sources in LAB.
6. Cross-link `ru/` ↔ `en/`.

Naming: `NNN-topic.md`, where NNN is the LAB experiment
number (e.g. `019-interaction.md`). For non-experiment
objects, use a short descriptive slug.

## Current contents

- `ru/019-interaction.md` — Experiment 019: first designed
  test of Interaction > Node. Zero R across all configurations.
  Methodological findings: transcript-control, dialogue vs
  transcript, anticipation.
- `en/019-interaction.md` — English mirror.

## Related documents

- `meta/context.md` (LAB) — strategic context: MAIA / LAB / CORPUS.
- `meta/method-interaction-addendum.md` (LAB) — H3 procedure.
- `meta/open-questions.md` (LAB) — open questions across LAB.
- `meta/changelog.md` (LAB) — history.
