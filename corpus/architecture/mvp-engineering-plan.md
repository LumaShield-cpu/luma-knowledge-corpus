# MVP engineering plan (execution detail)

**Source:** [SHIELD Architecture Series, Volume IV: Engineering Execution Blueprint](../../sources/docs/shield-architecture-series-volume-iv.pdf.meta.md).
Self-marked "Current Working Framework v0.2, Engineering Draft."

**Status: draft-tier, execution planning, not canon.** This is the
most implementation-specific of the Series volumes (repo structure,
tech stack options, dev environment, 30/60/90-day plan) — most of it
is the kind of detail that goes stale fast and isn't meaningfully
"canon." Captured here at lower fidelity than Volumes II/III; only the
scope/principle-level content is recorded.

## Engineering thesis

Build the smallest working system that proves the architecture, not
the full ecosystem. The MVP targets exactly two things: the Translation
Engine and Composition Engine, proven end-to-end against one real
artifact (reusing the [SmartTag Irving Oil case](translation-pipeline.md) —
same source, now as an engineering regression baseline rather than a
translation example).

## What the MVP explicitly is not

Full LumaShield consumer app, marketplace/distribution layer,
Professional Shield network, enterprise platform, mobile applications,
or "full AI operating system." Also **not**: replacing existing
enterprise systems, automating legal/medical judgment, training a new
foundation model, or eliminating human review from high-consequence
workflows. Framed explicitly as *sequencing* constraints, not
permanent limits — "each non-goal becomes a future goal once the MVP
evidence supports it."

## Twelve engineering principles

Consistent with (not additive beyond) what's already in
[decision 0004](../decisions/0004-constitutional-invariants.md) and
[translation-pipeline.md](translation-pipeline.md): evidence before
expansion, build from real artifacts (synthetic data for unit tests
only), preserve provenance as a schema requirement, keep Translation
and Composition as independent systems, stay model-agnostic, treat
connectors as governed/versioned assets, never embed secrets, validate
before publishing, version every schema, and treat every case study as
regression evidence.

## GEMS — the orchestration tool

**GEMS** ("the Shield Generator") is named as the orchestration layer
that drives the full pipeline end-to-end for a given organization —
from initial inputs (org name, website, source documents, goals) to
outputs (context package, knowledge graph, Shield spec, and prototype
generation prompts). Explicitly not required to be a polished product —
"a CLI tool, a Python notebook, or a simple web interface" is
sufficient for v0.1. It's a proof-of-concept implementation vehicle,
not a product in its own right.

## Outstanding named terms (not yet defined in this corpus)

This volume's own closing terminology table lists several canonical
terms this corpus hasn't independently reconciled yet:

- **HAIL** — tagged here as "interaction grammar, Volume III," but
  used elsewhere (the SmartTag case study in
  [translation-pipeline.md](translation-pipeline.md)'s source) as
  "HAIL Objects: canonical operational objects produced from Appenate
  controls" — these two usages don't obviously match; needs its own
  reconciliation pass once more source material exists.
- **Operational Self-Healing Layer** — named as a Volume II
  architecture component; not described anywhere in the material this
  corpus has ingested.
- **Luma ID** / **Shield ID** — named as identity systems from a
  "Volume I," but not the ARCH-02 Volume I already in this corpus
  (ARCH-02 never mentions either term) — confirms this Series has its
  own separate Volume I this corpus doesn't have.

## Status

Per this document's own words: *"Any apparent inconsistency between
Volume IV and prior volumes should be escalated to the Founder /
Product Architect for canon resolution before implementation
proceeds"* — i.e., even the Series' own authors treat internal
conflicts as needing human resolution, consistent with how this corpus
operates.
