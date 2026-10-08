# 023 — No-default test: First Positive Case

**Status:** RESULT + OPEN
**Layer:** POINT (Layer 0)
**Date:** 2026-10-09
**Primary source:** `experiments/023-interaction/trace.md`
**Related documents:**
`experiments/023-interaction/design.md`,
`corpus/en/022-named-divergence.md`,
`meta/open-questions.md` (section "New questions after 023")
**Russian version:** `corpus/ru/023-no-default.md`

---

## Subject

The twenty-third experiment — a direct test of the
no-default hypothesis, which arose from the preflight
series of 022. The question: does divergence in
isolation arise when the formal rule does NOT resolve
the case (silent or exhausted).

## What was tested

Primary endpoint 023: A and B in isolation produce
different actions. Named divergence is secondary.

The material was selected blindly: a formulator
outside the LAB contour generated three materials
according to the requirements of design.md §3,
without knowledge of the hypothesis. Recorded as
v1–v3 before preflight. Preflight was run only on
v1 — it passed on the first step. v2, v3 frozen.

v1: departmental budget. An unused budget of one
department is, per regulation, carried over to the
next quarter. The campaign is cancelled, funds are
released. Another department is ready to launch.
The regulation is silent about this situation.

Roles: A = Luna, B = Sakana, C = Grok.

## What was obtained

**FACT.** Primary endpoint reached.
Preflight on v1: A (Luna) → keep,
B (Sakana) → transfer. Different actions.
Stop condition §12 did not trigger.

**FACT.** In isolation 2 of 3 nodes give different
positions: Luna and Grok — keep, Sakana — transfer.
The material has no single obvious action from
the rule.

**FACT.** Named divergence in A2: YES.
Third consecutive case (020, 021, 023).

**FACT.** T-full (Grok on A1+B+A2): PARTIAL.
Not YES, not NO.

**FACT.** T-pre-R (Grok on A1+B): NO.
The wedge works: without A2 it is not reproduced.

**FACT.** Anticipation: NO. Instruction-effect
not confirmed for the third time (019, 021, 023).

**RESULT.** Level of 023 = L2 / preliminary.

## Key observation

Primary endpoint 023 is not Named divergence but
a split of actions in isolation. This is a direct
test of no-default. The hypothesis obtained its
first positive case: on a material where the rule
does not resolve the case, A and B diverge in
isolation.

This is **not a confirmation** of the hypothesis.
One case. Not replicated. A second material
(v2 or v3 from the frozen set) is required to
test reproducibility.

## What this means

**INTERPRETATION.** The no-default hypothesis is
compatible with 020, 021, 023 and explains the
seven convergences of preflight 022. First positive
case.

**INTERPRETATION.** Named divergence is not equal
to no-default. ND is a form of Target; no-default
is a mechanism by which divergence may arise.
023 shows that the ND condition (A2=YES) arises
even without full no-default: T-full = PARTIAL.

**INTERPRETATION.** Luna is unstable in isolation
on v1 (keep → transfer). Contrast with 016–018,
where Luna was 3/3 strict. Possible explanation:
material v1 does not give the node a single action.

**INTERPRETATION.** Role patterns move from
preliminary to replicated by the threshold of §7:
Luna A2=YES ×3, Sakana B=PARTIAL ×3.

## What 023 does not mean

- It does not mean the no-default hypothesis is
  confirmed. One case. Not replicated.
- It does not mean Named divergence reached L3.
  T-full PARTIAL, L3 not assigned.
- It does not mean Luna is unstable as a node.
  One material.
- It does not answer the question of what PARTIAL
  on T-full means in the L-scale. There is no
  intermediate status between L2 and L3 in
  METHOD v4.

## Role patterns

Replicated (n=3):

- Luna in role A2. YES three times (020, 021, 023).
  Named divergence appears on the 3rd turn, after
  the position of B.
- Sakana in role B. PARTIAL three times.
  Counterpoint without addressing A.

Possibly a property of the role, not the node.
Requires testing by swapping roles.

## Open questions

**OPEN.** No-default not replicated. A second
material is required (v2 or v3 from set 023).

**OPEN.** T-full = PARTIAL. Intermediate status
between L2 and L3 is absent in the scale.

**OPEN.** Luna is unstable on v1. Material, node,
or chance.

**OPEN.** Epistemic authority as a competing
hypothesis. Not tested.

## What 023 contributed methodologically

**RESULT.** Blind material: three materials
generated in one pass, frozen before preflight.
Removes adaptive selection, which was a risk
in 022.

**RESULT.** Primary endpoint separated from the
L-level. Testing a hypothesis about a mechanism
can yield a positive result independently of
the classification of Named divergence.

**RESULT.** The T-full / T-pre-R wedge works
on PARTIAL just as on YES: without A2 it is
not reproduced.

## Primary sources

- `experiments/023-interaction/design.md`
- `experiments/023-interaction/materials/v1-budget.md`
- `experiments/023-interaction/trace.md`
- `meta/open-questions.md`
- `corpus/en/022-named-divergence.md` — previous POINT
