# Related work — Positioning of LAB

**Status:** INTERPRETATION
**Layer:** POINT (Layer 0)
**Date:** 2026-10-08
**Primary source:** formulated by the lead based on
the accumulated context of LAB
**Related documents:**
`meta/context.md` (section 2),
`corpus/en/019-trajectory.md`,
`corpus/en/022-named-divergence.md`
**Russian version:** `corpus/ru/related-work.md`

---

## Subject

A brief positioning of NOVA CORTEX LAB relative to
adjacent lines of research. Not a literature review —
there are no bibliographic references here. It is a
description of what LAB does, what it does not do,
and what it can be confused with.

## What LAB investigates

The central question: can interaction between
independent LLM nodes produce something that is
present in none of them individually.

The hypothesis is formulated as: Interaction > Node.

Not "which model is better". Not "which answer is
correct". But: what appeared in the process of
interaction that cannot be fully reduced to the
initial material.

## Adjacent lines that LAB may intersect with

### 1. Multi-agent LLM systems

Field: dialogue of several LLM agents to solve tasks,
debate, role distribution.

Difference from LAB: the focus is not on the quality
of the task solution, but on the very fact that
something new emerges through interaction. Success
is measured not by "the best answer" but by
distinguishing interaction-effect from content-effect.

### 2. Emergent abilities in LLMs

Field: abrupt appearance of capabilities as model
size or data volume grows.

Difference from LAB: emergence is considered not
within one model but between models. Node capability
is not the subject of research; the subject is
interaction contribution on top of node capability.

### 3. Swarm intelligence and collective behavior

Field: homogeneous agents, local rules, global
pattern.

Difference from LAB: nodes are not homogeneous
(Luna, Sakana, Grok, Qwen — different models with
different profiles). The order of nodes is fixed.
Asymmetry is part of the design.

### 4. Aggregation and social choice

Field: preference collection, voting, weighted
aggregation.

Difference from LAB: not aggregation. LAB does not
sum up node answers and does not seek consensus.
The hypothesis is the appearance of something new,
not the reduction of something old.

### 5. Content-effect vs interaction-effect

Field: distinguishing the effects of communication
and content.

LAB contribution: transcript-control as a method of
distinction. A node receives the text of another
node without the ability to address it. If the
Target is reproduced — content-effect. If not —
interaction-effect.

## What LAB contributes methodologically

- Transcript-control as a content-transfer control.
- Preflight of Target reachability before the full
  battery.
- Distinction between Target-level and
  causal-mechanism-level.
- Named divergence as a form of Target.
- L0–L3 scale for classifying results.
- Negative result as a valid outcome
  (TARGET_MISS, OPEN).
- The no-default hypothesis: divergence requires
  a situation where the formal rule does not
  resolve the case. Working, not verified.

## What LAB does not do

- Not a benchmark. No comparison of models.
- Not SOTA. No race for the best result.
- Does not scale to n > 4 nodes (small contour,
  manual relay, one operator).
- Does not use top-tier models (access — free).
- Does not publish without CORPUS.
- Not a legal or banking infrastructure
  (a deliberate position).

## Limitations of positioning

- No bibliographic references. A literature review
  requires external contribution.
- Small n (4 nodes, 1 operator). Large conclusions
  are premature.
- External replication is absent. Everything LAB
  has done is reproducible within the contour but
  not independently confirmed.
- All results are preliminary if n is below the
  thresholds of §7 METHOD v4.

## Open questions

**OPEN.** Is a separate literature review with
bibliography needed, or is positioning by questions
sufficient for the current CORPUS layer.

**OPEN.** Is there an intersection with work in
HCI / multi-agent systems that LAB does not yet
take into account.

**OPEN.** How does the positioning change after
experiment 023 (validation of no-default), if
it takes place.

## Primary sources

- `meta/context.md`
- `corpus/en/019-trajectory.md`
- `corpus/en/020-named-divergence.md`
- `corpus/en/021-named-divergence.md`
- `corpus/en/022-named-divergence.md`
- `METHOD.md` (v4.0-rc1)
- `meta/method-interaction-addendum.md`
