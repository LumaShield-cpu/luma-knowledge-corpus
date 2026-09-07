# Reconciliation: "Core" (not "Pearl") is the current interaction primitive

**Date:** 2026-09-07
**Author:** Stacey (via reconciliation session)

## Conflict

Two naming families for the Shield's interaction primitives have been
recurring across sources:

- **Core / Ring / Pads / Dial / Adaptive Operational Briefing (AOB)**
  — from [shield-edge.pdf](../sources/docs/shield-edge.pdf.meta.md) and
  [ARC-01](../sources/docs/arc-01-shield-canonical-terminology-and-relational-architecture-v0.1.docx.meta.md)'s
  terminology dictionary. ARCH-02 §3.2 also names "Core... Adaptive
  Operational Briefing" by name (as things Volume I doesn't own),
  though ARCH-02 never itself defines these terms.
- **Shield / Context Window / Dial / Pads / Pearl / Ring** — with
  "Pearl" as the central confirmation/decision anchor and "Context
  Window" as the display-only layer. This family recurs across
  [Unified Canon State v3](../sources/docs/lumacanonos-unified-canon-state-v3.md)
  (uses "Window"), the
  [UI/UX Review](../sources/docs/lumashield-ui-ux-review.md) (mentions
  "Pearl" as an internal nickname for the center), the
  [SHIELD Constitution v2 outline](../sources/docs/shield-constitution-v2-2026-07-05.pdf.meta.md)
  (lists "Dial, Pads, Pearl, Ring" together under planned Volume IX),
  and
  [SHIELD Architecture Series, Volume II — Part II](../sources/docs/shield-architecture-series-volume-ii-part-ii.pdf.meta.md)
  (fully defines "Pearl: the central confirmation, continuation, or
  decision anchor. Confirms when evidence is complete and action is
  ready" — occupying the same conceptual role as "Core").

Both families recur across multiple independent-looking sources, which
is exactly the kind of ambiguity this corpus's own source-authority
rules warn against resolving by vote-counting alone (see
[CONTRIBUTING.md](../CONTRIBUTING.md) on AI self-corroboration not
counting as independent evidence — several of the "Pearl" sources may
themselves trace to the same underlying draft lineage rather than
being truly independent).

## Evidence

Direct confirmation from the product owner: **Core/AOB is current.
Pearl and Context Window are old, dropped naming.**

## Resolution

- **Core** is the correct term for the single highest-priority focal
  element / central confirmation anchor. "Pearl" is superseded — don't
  use it in new corpus content, and treat every "Pearl" reference in
  `sources/` as design history from a naming track that didn't survive.
- **Window** (or "Context Window") is superseded as a named primitive
  in its own right. Where a source describes a display-only,
  non-action layer, that concept now lives inside the Adaptive
  Operational Briefing / Semantic Experience Manifest framing rather
  than as a standalone "Window" primitive — see
  [enterprise-shield.md](../corpus/architecture/enterprise-shield.md).
  (If a distinct "context display" concept turns out still to be
  needed, that's a fresh design question, not a resurrection of
  "Window.")
- The "SHIELD Architecture Series" (Volumes II–V, all self-marked "Not
  Final Canon") appears to be a separate or earlier draft lineage from
  the one that produced ARCH-02 — its own "Volume I" description
  doesn't match ARCH-02's actual content, and none of ARCH-02 §20.2's
  named consolidation sources match this series' naming. Treat the
  Series as design history, consistent with ARCH-02's own
  tier-6 catch-all.

## Corpus update

- [corpus/architecture/shield-anatomy.md](../corpus/architecture/shield-anatomy.md) —
  "Pearl" footnote updated from "unverified naming, not promoted" to
  "confirmed superseded."
- [corpus/glossary.md](../corpus/glossary.md) — entry added pinning
  Core over Pearl.
