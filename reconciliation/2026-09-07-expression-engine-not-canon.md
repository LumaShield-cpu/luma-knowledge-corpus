# Reconciliation: the "expression engine" (Shield=Sentence) was never canon

**Date:** 2026-09-07
**Author:** Stacey (via reconciliation session)

## What happened

[Decision 0002](../corpus/decisions/0002-expression-engine.md) was
drafted straight into `corpus/` from
[Unified Canon State v3](../sources/docs/lumacanonos-unified-canon-state-v3.md),
which repeatedly and confidently asserts a grammatical mapping (Shield =
Sentence, Pads = Verbs, Signals = Meaning, Protocols = Execution, People
= Subjects) as locked canon. The same mapping also appears in
[LumaOS Cold Ingestion](../sources/docs/lumaos-cold-ingestion.md) item
[003], which was cited as independent corroboration — multiple sources
agreeing looked like a strong signal.

## Conflict

Direct correction from the product owner: **this was never an actual
product decision.** It's a rhetorical framing device the AI kept
generating across separate chat sessions — a favorite way for the model
to describe the system, re-asserted confidently each time it came up,
not something the team ever discussed, decided, or locked.

## Why the "corroboration" was worthless here

This is the important lesson: **two documents both being ChatGPT output
is not two independent sources.** Corroboration is only meaningful when
it comes from sources that could plausibly disagree — different
authors, different sessions grounded in different evidence, human
ratification, actual shipped behavior. Two chats with the same model,
neither grounded in anything outside the model's own prior outputs, can
agree with each other endlessly without that agreement meaning
anything. The model repeating its own idea back convincingly is not
evidence the idea is real.

This generalizes: every "corroboration" claim already made or still to
be made in this corpus should be checked for what's actually on the
other end of it — a different, grounded source, or just the same
generator talking to itself again.

## Resolution

Decision 0002 is rejected, not canon, and must not be cited. It is left
in place (marked REJECTED) rather than deleted, per this project's
practice of keeping mistakes on the record rather than erasing them.

Corpus references to it were removed: system-layers.md (since moved
to shield-canon as part of the Luma/Shield split) no longer cites it
and no longer describes Luma via the Sentence/Verb framing.

## Open question

If there's a real, actually-decided model for how Shield/Pads/Signals/
Protocols relate to each other (as opposed to this rhetorical one), it
hasn't been identified yet in this corpus. Until it is, `corpus/`
describes these elements individually (see
[architecture/shield-anatomy.md](../corpus/architecture/shield-anatomy.md))
without asserting an overarching grammar.

## Corpus update

- [corpus/decisions/0002-expression-engine.md](../corpus/decisions/0002-expression-engine.md) — marked REJECTED.
- system-layers.md (since moved to shield-canon) — reference removed, rewritten.
