# Reconciliation: shield-canon is out of this corpus's authority scope

**Date:** 2026-09-07
**Author:** Stacey (via reconciliation session, with cross-session
investigation by a peer Claude session working directly in
`github.com/Solid-Stride/shield-canon`)

**Final ruling, direct quote from the product owner (relayed via the
peer session):** *"shield canon is separate and peer is working on
reconciliation."* This means shield-canon was never actually a
candidate for this corpus's authority hierarchy — not a conflict that
got resolved with an exception, but a system outside this corpus's
jurisdiction entirely. It's recorded below as a scope note, not a
conflicts-found record, though the individual findings are kept for
reference since (b) and (c) are still useful facts to have on hand.

## Background

While reconciling the SHIELD Architecture Series, a separate repo —
`shield-canon` — was discovered to exist as "its own project." A peer
session was opened directly in that repo and grepped it exhaustively
for every term this corpus needed (HAIL, IADR, SCK, AMC, HRD, ARCH-02,
"Volume I", Pearl, Edge, Self-Healing, Luma ID, Shield ID): **zero
hits for all of them.** shield-canon has no lineage back to ARCH-02 or
the Architecture Series — it's an independently-rooted repo (10
commits, all 2026-07-07–2026-09-06, three distinct author identities
including a machine author, "Copilot App," on its APPROVED token
file — nothing hash-bound or signed).

Three things surfaced instead:

## (a) Two independent "Constitutions" — RESOLVED, not a conflict

`01_CONSTITUTION/LAWS.md` in
[github.com/Solid-Stride/shield-canon](https://github.com/Solid-Stride/shield-canon)
declares itself supreme authority within its own repo, with no
reference to ARCH-02 or any Series volume. (Verbatim text was relayed
via a peer Claude session working directly in that repo, then reviewed
here — not kept as a local copy, since shield-canon is confirmed out
of this corpus's scope; see the repo itself for the current text.)

**Resolution:** confirmed by the product owner —
shield-canon is deliberately, separately scoped. **LumaShield is
free, public, personal-use software; "Shield" (unqualified) is the
professional/business tier and up.** shield-canon is LumaShield's own
design-system canon, not a competing claim on the broader SHIELD
architecture's authority. Not a drift incident — see the product-tier
note added to
[corpus/architecture/system-layers.md](../corpus/architecture/system-layers.md).
This is the same kind of scoping already established for the
[four-Pad Shield layout](../corpus/architecture/shield-anatomy.md):
LumaShield can make its own product-level choices without those
choices being universal SHIELD law.

## (b) Red as a canon color in shield-canon — RESOLVED: allowed

`03_VISUAL_GRAMMAR/DESIGN_TOKENS.md` in shield-canon (self-marked
APPROVED) defines `color.action.danger` and `color.state.error` as
`#E5484D` (red) — the **only** token available for either semantic
(its own Usage Rule 1 makes the token set exclusive). This was
confirmed verbatim (relayed by the peer session, not paraphrased) at
the time of this reconciliation.

This is narrower than first reported: an initial claim that
`10_EXAMPLES/login-form.md` self-certified compliance while visibly
using red was checked by the retrieving session and **retracted** —
that file's compliance checklist has no color check at all. The red
"conflict" lives entirely in `DESIGN_TOKENS.md`.

**Resolution, confirmed by the product owner:** allowed. The "Red is
forbidden" rule (established at the broader SHIELD/Architecture-Series
doctrine level — see [decision 0003](../corpus/decisions/0003-glow-system.md))
does not bind LumaShield's separately-scoped design system, on the same
precedent as the [four-Pad layout](../corpus/architecture/shield-anatomy.md).
Decision 0003 has been annotated accordingly. **Do not treat this as
license to relax the red-ban anywhere else** — it applies specifically
to LumaShield's own product design system, per its separate scoping,
not as a general softening of the rule.

## (c) Overlapping forbidden-term lists — convergent, not conflicting

shield-canon's Law 3 bans "dashboard, page, menu, navigation, card,
board, portal" in canonical documentation, stated rationale: "these
terms promote cognitive patterns that contradict SHIELD design
principles." This independently arrives at the same doctrine already
in this corpus ("SHIELD Is Not a Dashboard,"
[0006's anti-patterns list](../corpus/decisions/0006-interaction-doctrine-detail.md)
naming "Dashboard Overload" and "Menu Sprawl") without citing it.
**Not a conflict** — two documents reaching the same rule
independently. Worth noting as evidence the doctrine propagated
informally between the two efforts, even without a shared citation
trail.

## Also flagged (not yet acted on)

- `daily-truth-build.yml` in shield-canon runs a cron that
  auto-commits `_build/DAILY_CANON_DIFF.md` and
  `_build/LATEST_DECISIONS.md` — per the retrieving session, both are
  written via a quoted heredoc that emits `$(date)` literally, so these
  are **stub files with empty boilerplate bodies**, not a real decision
  log. If either is ever ingested as a source, treat as unverified.
- An unread branch, `lumashield-cpu-agent-governance-standard`, was
  flagged by the peer session as the most plausible place (within
  shield-canon) for anything resembling a "Volume I" — not yet checked.

## Corpus update

- [corpus/architecture/system-layers.md](../corpus/architecture/system-layers.md) —
  added the LumaShield (free/personal) vs. Shield (professional/
  business+) product-tier distinction. (This doc has since moved to
  shield-canon as part of the broader-Shield/Luma corpus split —
  2026-09-07 — but the product-tier fact it recorded remains true.)
- [corpus/decisions/0003-glow-system.md](../corpus/decisions/0003-glow-system.md) —
  annotated with the LumaShield/shield-canon red exemption.
- The three shield-canon files (LAWS.md, DESIGN_TOKENS.md, the
  login-form excerpt) were briefly ingested verbatim with full git
  provenance for this reconciliation, then removed once shield-canon
  was confirmed out of scope — they're redundant with the actual repo,
  which is the citable source going forward.
