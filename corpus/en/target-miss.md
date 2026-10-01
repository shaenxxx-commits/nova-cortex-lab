# TARGET_MISS — A Fourth Class of Outcome

**Status:** INTERPRETATION + HYPOTHESIS
**Layer:** POINT (Layer 0)
**Date:** 2026-09-30
**Primary source:** `experiments/019-interaction/trace.md`
(L3 Check, Level Assignment)
**Related documents:**
`meta/method-interaction-addendum.md` §11,
`corpus/en/019-interaction.md`
**Russian version:** `corpus/ru/target-miss.md`

---

## Subject

METHOD v4 and the addendum describe three classes
of outcome for an interaction experiment:

- **H1 YES** — Target is accessible in isolation.
- **H3 not supported** — Target exists in dialogue,
  but is reproduced in isolation or transcript-control.
- **content-effect** — Target is reproduced
  from the transmitted material.

Experiment 019 revealed a **fourth case**:
Target did not appear **anywhere**. Not in dialogue,
not in isolation, not in transcript, not in anticipation.

This is TARGET_MISS.

## What this means

**INTERPRETATION.** TARGET_MISS is not "interaction
does not work". It is a signal of incompatibility
between the Target and the material or the task.

The distinction is fundamental:

- Under "H3 not supported", Target exists but does not
  require interaction. The test was run; the answer is
  negative.
- Under TARGET_MISS, Target does not appear at all.
  There was nothing to test. H3 was not tested.

## How it differs from neighbouring classes

**FACT.** In 019, R did not appear in any configuration:

| Configuration | R |
|---|---|
| Dialogue A↔B (3 turns) | no |
| C on transcript | no |
| Isolation (Luna, Sakana, Grok, n=2) | no |
| Transcript-control (B, C) | no |
| Anticipation (Luna) | no |
| Qwen (confounded) | no |

**INTERPRETATION.** This is not H1 YES: Target
did not appear even in isolation.

Not H3 not supported: there is nothing for H3 to
refute, Target did not appear in dialogue.

Not content-effect: Target is not reproduced
from material, because it is not in the material.

Not a "null result" in the sense of L0: nodes produced
substantive answers, but not toward the Target.

## Action on TARGET_MISS

**HYPOTHESIS.** When TARGET_MISS is detected:

- Do not reclassify the experiment post hoc.
- Do not weaken the criteria (A1, scale).
- Change the Target in the next experiment.
- Run a Target-reachability preflight
  (see `meta/method-interaction-addendum.md` §12):
  1–2 isolation runs on a draft Target
  before the full battery.

## Possible causes of TARGET_MISS

**HYPOTHESIS.** Dominant interpretation
from external review of 019: Target/material mismatch.
The material systematically pushes nodes toward
rejecting the framing of the task.

**HYPOTHESIS.** Alternative: Target was too strict
in form. A1 requires an operational switching rule
"under X → [i], under Y → [j]".
No node produced such a form.

In 019 these two hypotheses are not distinguishable.

## What this does not mean

- It does not mean interaction cannot produce a Target.
  This cannot be tested with 019 — the Target did not
  appear anywhere, there was nothing to compare.
- It does not mean the addendum procedure fails.
  The procedure worked end-to-end; the discovery of
  TARGET_MISS is its result.
- It does not mean TARGET_MISS is a final class.
  This is a working notion, introduced after one case.

## Open questions

**OPEN.** TARGET_MISS as a class is anchored on a single
case. A second case is required: an interaction
experiment with a different Target, where R either
appears or again does not appear.

**OPEN.** Whether TARGET_MISS should be a mandatory
field in the trace format for interaction experiments.
It is currently a description in addendum §11.

**OPEN.** Formal relationship to METHOD v4 §7.
TARGET_MISS is absent from METHOD v4. Integration —
after the second case.

## Primary sources

- `experiments/019-interaction/trace.md` —
  sections L3 Check, Level Assignment, Operator Notes
- `meta/method-interaction-addendum.md` §11 —
  definition of TARGET_MISS
- `corpus/en/019-interaction.md` — general POINT on 019
- `corpus/en/transcript-control.md` — POINT on
  transcript-control
