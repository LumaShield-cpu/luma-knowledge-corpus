# Decision 0002: The expression engine — Luma as a coordination language

> **REJECTED 2026-09-07 — not canon.** This was never an actual product
> decision. It's a recurring rhetorical framing the AI itself kept
> re-asserting across separate chat sessions — which is why it looked
> corroborated by "independent" sources below. Those sources aren't
> independent: they're the same model restating its own prior framing,
> not separate human ratification. See
> [reconciliation/2026-09-07-expression-engine-not-canon.md](../../reconciliation/2026-09-07-expression-engine-not-canon.md).
> Left in place, not deleted, as a record of the mistake. Do not cite
> this doc as canon.

**Status:** ~~Locked~~ REJECTED — see notice above.
**Source:** [Unified Canon State v3](../../sources/docs/lumacanonos-unified-canon-state-v3.md), §2.1.
**Corroboration:** the same mapping appears independently in earlier
extraction passes over separate source material — e.g.
[LumaOS Cold Ingestion](../../sources/docs/lumaos-cold-ingestion.md)
item [003] — which strengthens confidence this wasn't a one-off framing.

## Context

Earlier system thinking (v2) treated actions, signals, and protocols as
overlapping, loosely-defined concepts — useful ideas that hadn't
crystallized into a single consistent model. This made the system hard
to describe precisely for engineering or patent purposes.

## Decision

Luma is defined as a **coordination language**, with a fixed grammatical
mapping:

| Luma element | Grammatical role |
| --- | --- |
| Shield | Sentence |
| Pads | Verbs |
| Signals | Meaning |
| Protocols | Execution |
| People | Subjects |

This is the foundational grammar referenced by every other doctrine
(interaction, glow, packets) — those are all expressions of this
underlying language, not independent systems bolted together.

## Consequences

- Luma should be described and pitched as a *language*, not "an
  interface" or "an app" — this affects patent framing, product
  positioning, and how new features get evaluated (does this fit the
  grammar, or does it strain it?).
- New system elements should be checked against this mapping before
  being added: if something doesn't clearly map to Sentence / Verb /
  Meaning / Execution / Subject, that's a signal it may not belong at
  this layer, or the mapping itself needs a reconciliation review.
