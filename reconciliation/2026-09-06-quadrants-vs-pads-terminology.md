# Reconciliation: "quadrants" vs "pads" terminology

> **SUPERSEDED 2026-09-06.** This record's resolution was wrong — it
> was based on an unverified verbal answer, given before the primary
> source (`lumacanonos-unified-canon-state-v3.md`) had been located and
> checked. See
> [2026-09-06-quadrants-vs-pads-terminology-corrected.md](2026-09-06-quadrants-vs-pads-terminology-corrected.md)
> for the corrected resolution. Left in place, rather than rewritten,
> as a record of how this went wrong the first time.

**Date:** 2026-09-06
**Author:** Stacey (via reconciliation session)

## Conflict

An earlier automated extraction pass ([sources/docs/lumaos-data-extraction.md](../sources/docs/lumaos-data-extraction.md),
items [052]–[053], [115]–[116]) flagged "quadrants" and "pads" as
conflicting terms for the same shield element — the four selectable
action zones around the shield's center. One extracted note even reads
"Quadrant Pad Dimensions," mixing both terms in a single phrase. Other
sources use the terms inconsistently:

- [sources/docs/luma-shield-documentation.md](../sources/docs/luma-shield-documentation.md)
  (a system prompt for canon documentation) uses "quadrants" throughout
  ("ICON LAW," "Icons exist only inside quadrants").
- [sources/docs/lumashield-ui-ux-review.md](../sources/docs/lumashield-ui-ux-review.md)
  (a later, dated UI/UX canon snapshot) uses "pads" ("4 surrounding
  pads/quadrants").
- [sources/docs/lumaos-cold-ingestion.md](../sources/docs/lumaos-cold-ingestion.md)
  item [002] explicitly states: "We changed quadrants to pads. Correct
  language" — read in isolation, this looks like a full terminology
  replacement.

## Evidence

Direct confirmation from the product owner: this was never a
replacement — it's two names for the same structure, used in different
registers.

## Resolution

Not a conflict. Both terms are correct, scoped by audience:

- **"Quadrants"** — the technical/internal term, used in engineering,
  patent, and architecture documentation.
- **"Pads"** — the marketing/public-facing term, used in user-facing
  copy, UI/UX documentation, and external communication.

The item [002] note ("we changed quadrants to pads") describes the
introduction of the public-facing term alongside the existing technical
one, not a deprecation of "quadrants."

## Corpus update

Added an entry to [../corpus/glossary.md](../corpus/glossary.md) pinning
both terms and their scopes.
