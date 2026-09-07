# Contributing to the corpus

The core rule: **nothing lands in `corpus/` without a reconciliation record
justifying it**, unless it's genuinely uncontested (see "Fast path" below).
That's what keeps this repo from drifting the same way the last set of docs
did.

## 1. Bring in a source

Drop raw material into the matching `sources/` subfolder exactly as found —
don't clean it up or summarize it yet. At the top of the file (or in a
sibling `.meta.md` if the source is a non-text format), note:

- Where it came from (URL, ticket ID, export, person)
- Date pulled
- Date the original was authored/last updated, if known

## 2. Check it against reality

Before trusting anything a source claims, check it against current behavior
(running code, actual configuration, actual data) and against other
sources. Three outcomes:

- **Confirmed, uncontested** — no other source disagrees and it matches
  reality. Skip to the fast path below.
- **Conflicting** — two sources disagree, or a source disagrees with
  `corpus/`, or a source disagrees with observed reality. Open a
  reconciliation record.
- **Stale/dead** — the source describes something no longer true and
  nothing depends on knowing the old state. Note it as superseded in the
  source file itself; it does not need a corpus entry.

## 3. Reconciliation record

Copy `reconciliation/template.md` into a new dated file
(`reconciliation/YYYY-MM-DD-short-topic.md`) and fill it in: what conflicted,
what evidence settled it, what the actual answer is now. Append a one-line
entry to `reconciliation/log.md` linking to it.

## 4. Update the corpus

Write or update the canonical doc under `corpus/` in plain, current-tense
language — describe what *is* true, not the history of how it became true.
Link back to the reconciliation record (or, for the fast path, directly to
the source) so anyone can see the evidence trail.

## Fast path

For a genuinely uncontested fact (one source, matches reality, nothing to
reconcile), you can write directly to `corpus/` citing the source — no
reconciliation record needed. If you're not sure it's uncontested, it isn't;
write the record.

## Cross-repo governance

As of 2026-09-07, Stacey has confirmed that **`SHIELD_AGENT_OPERATING_STANDARD.md`
becomes the umbrella governance standard for this repo, shield-canon,
and future repos** in this ecosystem. It's currently on an unmerged
branch in `github.com/Solid-Stride/shield-canon`
(`lumashield-cpu-agent-governance-standard`), human-authored by Stacey
Malitowski on 2026-07-17 — not yet citable at a stable path/commit
here, but the adoption decision itself is confirmed and effective now.

Notably, its authority hierarchy, its "never choose silently between
conflicting canonical sources" rule, its ban on rewriting approved
language without authorization, and its rule to log a specification
gap rather than invent one, all **independently converged** with this
repo's own `reconciliation/` process and source-authority rules below —
built without either side knowing the other existed. Once the standard
is merged and stably citable, this file should be updated to reference
it directly and defer to its authority hierarchy where the two might
ever diverge; until then, treat this file's own rules as consistent
with, not competing against, that standard.

## Source authority

Not all sources are equal, and recency does not automatically win. In
particular: a
[known corrupting event](reconciliation/2026-09-06-full-system-reset-non-authoritative.md) —
a "Full System Reset" that told a chat session to treat no prior canon
as locked — sits in the middle of this project's history. Material
generated only *because* that reset told a session to reinvent
definitions from scratch is not automatically trustworthy just because
it's more recent than what it reset. When weighing conflicting sources,
prefer whichever side is independently corroborated over whichever side
is newer.

**"Independently corroborated" means grounded in something that could
plausibly disagree** — a different author, a different session grounded
in different evidence, human ratification, or actual shipped behavior.
Two ChatGPT sessions agreeing with each other is not corroboration if
neither is grounded in anything but the model's own prior output — it
may just be the same generator confidently restating its own earlier
framing (see
[reconciliation/2026-09-07-expression-engine-not-canon.md](reconciliation/2026-09-07-expression-engine-not-canon.md)
for a case where this fooled a reconciliation pass). Before citing
"multiple sources agree" as evidence, check what's actually generating
each source.

### Translation Engine / Volume I matters — now out of scope here

ARCH-02 (the formal Translation Engine, Volume I architecture) and its
own ranked source-authority hierarchy moved to
[shield-canon](https://github.com/Solid-Stride/shield-canon) as part
of the Luma/Shield split — this repo no longer holds Volume I content
or needs to reproduce that hierarchy. If a question actually concerns
Translation Engine / Volume I architecture, it belongs in shield-canon,
not here. This repo's own material is LumaShield-scoped; use the
general corroboration rule above for it, and defer to shield-canon
entirely for anything broader-Shield.

## Conventions

- `corpus/` docs are living — edit in place as truth changes, don't fork
  "v2" copies. Git history is the changelog.
- `sources/` files are immutable once added — if a source turns out wrong,
  that's exactly what a reconciliation record is for, not an edit to the
  source.
- Prefer many small, single-topic docs in `corpus/` over few large ones —
  easier to keep individually correct.
