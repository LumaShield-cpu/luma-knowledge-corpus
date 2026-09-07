# Reconciliation: Luma's model class — LLM vs. SLM

**Date:** 2026-09-07
**Author:** Stacey (via reconciliation session)

## Conflict

shield-architecture-update-002.pdf (since moved to shield-canon as
part of the Luma/Shield split) is marked **APPROVED** and states:

> This update supersedes earlier assumptions that Luma itself was an
> LLM, establishing instead that Luma is the persistent personal
> intelligence layer of the SHIELD ecosystem.

This reads as settling the question — but it only tells us what Luma
*isn't* (an LLM) and what role it plays (persistent personal
intelligence layer), not what kind of model actually powers it.

## Evidence

Direct clarification from the product owner, given immediately after
this document was ingested: **the "not an LLM" framing has since
changed to "an SLM"** — a Small Language Model — rather than being
merely a role description with the model class left open.

## Resolution

Luma runs on (or is characterized as) an **SLM (Small Language
Model)**, not an LLM. This is a further evolution on top of what
Update 002 itself already established, not a contradiction of it —
Update 002 correctly ruled out "LLM," this correction fills in what
the actual answer is.

## Corpus update

No corpus doc exists yet describing what Luma is or runs on — this
should be captured when one is written (a `corpus/architecture/` or
`corpus/decisions/` doc on Luma's model architecture), rather than
retrofitted here. Flagging this record as the citation for "SLM, not
LLM" when that doc is drafted.

## Note on document currency

This is a second instance (after the pads/quadrants correction) of a
formally approved document already being one step behind current
reality by the time it was ingested. Approval status describes the
document's own conformance, not a guarantee that nothing has moved
since — check with the product owner before treating an "APPROVED"
document as necessarily current, especially on fast-moving specifics
like model choice.
