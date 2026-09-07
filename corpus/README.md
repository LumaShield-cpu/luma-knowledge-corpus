# corpus/

Canonical, current-truth knowledge about Luma. If it's here, treat it as
true today. If you find something here that's wrong, that's drift starting
again — fix it and, if it conflicts with something else on record, open a
reconciliation record (see [../CONTRIBUTING.md](../CONTRIBUTING.md)).

## Layout

- `architecture/` — how the system is actually built and how its pieces fit
  together, as it stands today (not as originally designed).
- `decisions/` — durable decisions and the reasoning behind them (ADR-style:
  one file per decision, context/decision/consequences). Once written, a
  decision doc doesn't get deleted when superseded — it gets marked
  superseded and links to what replaced it.
- `features/` — what each feature actually does today, from a user- or
  system-behavior point of view, not what a spec once proposed.
- `glossary.md` — terms that have drifted or been used inconsistently,
  pinned to one meaning.

## Ground rules

- Write in present tense, describing current reality.
- Every claim should be traceable to a source or reconciliation record —
  cite it (link or filename) rather than asserting from memory.
- If you're not sure something is still true, it doesn't belong here yet —
  move it to `sources/` and go through reconciliation.
