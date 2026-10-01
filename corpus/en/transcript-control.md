# Transcript-control as a Content-transfer Control

**Status:** RESULT + OPEN
**Layer:** POINT (Layer 0)
**Date:** 2026-09-30
**Primary source:** `experiments/019-interaction/trace.md`
(runs Transcript B, Transcript C)
**Related documents:**
`meta/method-interaction-addendum.md` §4,
`corpus/en/019-interaction.md`
**Russian version:** `corpus/ru/transcript-control.md`

---

## Subject

Transcript-control is one of the key controls in the H3
(interaction contribution) verification procedure.
Its purpose is to distinguish **interaction-effect**
from **content-effect**.

The question it answers: if a node receives not a live
interaction but a ready-made text of a previous response,
will it reproduce the Target?

- If yes — the Target does not require interaction, it
  requires content. H3 is not supported.
- If no — there is a signal that interaction adds
  something to the transmitted material.

## How it was run in 019

Two runs on the main line:

- **Transcript B.** Sakana receives the text of Luna A1
  as material. No feedback from the author,
  no knowledge of the dialogue.
- **Transcript C.** Grok receives the texts of Luna A1
  and Sakana B as materials. Same mode.

Comparison with dialogue: in dialogue, Sakana and Grok
knew their response would be received by another node
and that the other would respond. In transcript — they
only knew they were working with text.

## What was obtained

**FACT.** Sakana on the transcript of Luna A1 reproduced
its structure almost verbatim: the same four levels
(subject / artifact / content / basis),
the same 9 axes of source assessment.

**FACT.** Grok on the transcript of A1 + B reproduced
the same structure. The same 9 axes.

**FACT.** In dialogue, the same nodes produced **their
own** moves: Sakana — "reliability regimes", Grok —
"epistemic tracing". Not reproduction of the material.

## What this means

**RESULT.** Transcript-control works as a
**content-transfer control**. A node receives material
and passes its structure on. This is confirmed
on two nodes.

**RESULT.** Dialogue and transcript are distinguishable
by result. With the same initial input:

- in dialogue, nodes produce their own moves;
- in transcript — they reproduce the structure
  of what was transmitted.

This means: the interaction format influences
the *type* of response, not only its content.

## Limitation

**OPEN.** The H3-discriminating capability of
transcript-control (to distinguish an interaction-only
Target from reproduction of material) has **not been
tested on a positive Target case**.

019 did not provide a positive case: Target R
did not appear anywhere — not in dialogue, not
in isolation, not in transcript. There was nothing
to test.

Strict validity requires an experiment in which:

- Target is present in dialogue;
- Target is absent in isolation;
- Target is not reproduced in transcript-control.

Until such a case is obtained, transcript-control
is considered working as content-transfer, but
not as a full H3-control.

## What this does not mean

- It does not mean transcript-control is unimportant.
  It is important precisely as content-transfer:
  without it, one cannot distinguish interaction
  from content transmission.
- It does not mean dialogue is "stronger" than
  transcript. The result of 019 is about distinguishability
  of formats, not about superiority.
- It does not mean an interaction-effect was found.
  R did not appear anywhere; there was nothing
  to compare.

## Open questions

**OPEN.** How to measure proximity of a response
to the material? A coarse `HIGH_COPY` / `TRANSFORM`
metric was proposed in external review, not implemented.

**OPEN.** Possible artifact: an LLM's tendency to copy
well-structured text. A negative probe (transcript
with shuffled or truncated material) was proposed,
not implemented.

**OPEN.** A positive Target case is needed. Planned
for 020.

## Primary sources

- `experiments/019-interaction/trace.md` —
  runs `Transcript B — Sakana`, `Transcript C — Grok`
- `meta/method-interaction-addendum.md` §4 —
  definition of transcript-control and status after 019
- `corpus/en/019-interaction.md` — general POINT on 019
