# 021 — Named divergence: Second Attempt and Its Result

**Status:** RESULT + OPEN
**Layer:** POINT (Layer 0)
**Date:** 2026-10-05
**Primary source:** `experiments/021-interaction/trace.md`
**Related documents:**
`meta/method-interaction-addendum.md` §14,
`corpus/en/020-named-divergence.md`
**Russian version:** `corpus/ru/021-named-divergence.md`

---

## Subject

The twenty-first experiment — the second test of Named
divergence. The first, 020, gave L3 / INTERACTION-ONLY
(n=1). The goal of 021 was to reproduce the result on
a different material and lift `replication pending`.

The first experiment on METHOD v4.0-rc1
(provisional freeze).

## What was tested

Target (R): Named divergence — a node explicitly states
where its position diverges from the position of another
node, names the divergence and justifies it.

Material: a concrete case. Medical triage: two victims,
one operating room. One is young with a high prognosis;
the other is elderly with a low prognosis but was
delivered first.

Form — same as 019 and 020:
A1 -> B -> A2 + C on transcript + isolation
+ transcript-control + anticipation.

## What was obtained

**FACT.** R appeared in two runs:

- Dialog A2 (Luna): YES.
- Dialog C (Grok on full A1+B+A2): YES.

**FACT.** R did not appear:

- 6 isolation (Luna, Sakana, Grok x 2): all NO.
- Transcript B (Sakana on A1): NO.
- Transcript C (Grok on A1+B, without A2): NO.
- Anticipation (Sakana): NO.

**RESULT.** Level of 021 = L2 / preliminary.

**FACT.** The INTERACTION-ONLY condition is violated:
R is reproduced in transcript-control (C on full
A1+B+A2).

## What this means

**INTERPRETATION.** 021 is not a second L3. The
INTERACTION-ONLY condition is not met.

**INTERPRETATION.** Named divergence is not
INTERACTION-ONLY as a class. 020 showed one mode,
021 another. One Target-class, different reproduction
modes.

**INTERPRETATION.** Target-level != causal-mechanism-level.
Named divergence is a form of Target. INTERACTION-ONLY
is one possible mechanism for R.

**INTERPRETATION.** A2-dependence: content-effect
requires a ready formulation of R in the text of A2.
Without A2 (Dialog C on A1+B) — R is not reproduced.

## Key finding

Difference between two transcript-control runs:

| Run | What C saw | R |
|---|---|---|
| Dialog C | A1 + B + A2 | YES |
| Transcript C | A1 + B | NO |

The only difference is the presence of A2. Content-effect
depends on the ready formulation of the Target in A2.

This is called the T-full / T-pre-R wedge.

## What 021 does not mean

- It does not mean 020 was misclassified. 020 remains
  L3 / preliminary. Not downgraded.
- It does not mean Named divergence is a bad Target.
  It transfers. But causal classification does not
  transfer automatically.
- It does not mean interaction does not work.
  Interaction gave R in A2. Then R was transmitted
  through the transcript.

## Role patterns

Preliminary (n=2):

- Luna in role A2. YES twice (020, 021).
  Named divergence appears on the third turn, after
  the position of B.
- Sakana in role B. PARTIAL twice (020, 021).
  Counterpoint without addressing A.

Possibly a property of the role, not the node.
Requires testing by swapping roles.

## Open questions

**OPEN.** Downgrade 020 to L2 or keep L3 with the n=1
caveat? Position of the lead: keep. External observers
(Luna, Grok) agree. One voice (Kimi) for downgrade.

**OPEN.** Continue Named divergence (022) or change
the Target? Position: continue, but with a clarifying
design.

**OPEN.** Is T-pre-R a criterion or diagnostics?
After review: diagnostics, not a level criterion.

## What 021 contributed methodologically

**RESULT.** Three results:

1. First experiment on v4.0-rc1. Provisional freeze
   observed. No amendments to METHOD during the run.
2. Anticipation applied for the first time. NO.
   Instruction without interaction does not give R.
   Instruction-effect not confirmed.
3. T-full / T-pre-R wedge. A diagnostic tool for
   separating content-effect from A2 and content-effect
   from the full transcript.

## Primary sources

- `experiments/021-interaction/input.md`
- `experiments/021-interaction/trace.md`
- `meta/method-interaction-addendum.md` §14
- `corpus/en/020-named-divergence.md`
