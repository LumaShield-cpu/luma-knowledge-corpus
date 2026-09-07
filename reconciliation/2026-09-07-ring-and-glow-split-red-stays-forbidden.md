# Reconciliation: Ring and Glow are distinct elements; Red stays forbidden

**Date:** 2026-09-07
**Author:** Stacey (via reconciliation session)

## Conflict

[SHIELD Architecture Series, Volume III](../sources/docs/shield-architecture-series-volume-iii.pdf.meta.md)
(self-marked "Design Doctrine Draft") introduced two points of tension
with [decision 0003](../corpus/decisions/0003-glow-system.md) (sourced
from V3 + Luma Shield Documentation, two-source corroborated):

1. **Structure:** Volume III treats "Ring" (§11 — discrete operational
   state, structured expression) and "Glow" (§12 — ambient
   emotional/character layer, continuous, peripheral) as two separate
   grammar elements. The existing corpus decision treats them as one
   ("Glow State Ring").
2. **Color canon:** Volume III's color canon (§13) includes **Red** as
   a real, meaningful signal ("critical risk, invalid state, urgent
   stop") — directly contradicting decision 0003's "Red and green are
   explicitly forbidden." It also reassigns some existing colors'
   meanings (e.g. White as "human judgment/resolution" rather than
   "Idle"; Violet as "watch/concern/protective" rather than
   "Action/response").

## Evidence

Direct confirmation from the product owner on both points:
- **Ring and Glow are genuinely distinct elements** — Volume III is
  right, the existing corpus's merged framing was incomplete.
- **Red remains forbidden** — Volume III is wrong on this specific
  point; the existing decision 0003 color canon stands.

## Resolution

- **Structural split adopted:** Ring (discrete, structured operational
  state — connected/in-progress/blocked) and Glow (continuous, ambient
  emotional/character layer — the felt quality of the current moment)
  are now documented as two elements, not one, in
  [decision 0003](../corpus/decisions/0003-glow-system.md).
- **Color canon NOT changed:** the existing four colors and their
  meanings (White = Idle, Teal = Presence, Amber = Attention, Violet =
  Action) and the red/green prohibition remain as previously
  reconciled. Volume III's Red-inclusive canon and its alternate
  meanings for White/Violet are not adopted.
- Volume III's specific named Glow *states* (Calm Presence, Active
  Coordination, Watch State, Action Required, Concern, Completion) are
  plausible additive detail — they describe situations, not new colors
  — but are not independently re-verified here. Treat them as
  draft-tier illustrative examples, not confirmed canon, pending a
  closer pass if they matter for implementation.

## Corpus update

[corpus/decisions/0003-glow-system.md](../corpus/decisions/0003-glow-system.md)
restructured into two sections (Ring, Glow) under the existing color
canon, with Volume III's Red-inclusive version noted and rejected.
