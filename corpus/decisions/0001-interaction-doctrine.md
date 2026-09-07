# Decision 0001: Interaction doctrine — one screen, state-based, one tap or it fails

**Status:** Locked (per source; not yet re-confirmed against current build)
**Source:** [Unified Canon State v3](../../sources/docs/lumacanonos-unified-canon-state-v3.md), §3, §5.

A fuller, independently-corroborating version of this doctrine (twelve
design laws, anti-patterns, a concrete onboarding metric) has moved to
the [shield-canon](https://github.com/Solid-Stride/shield-canon) repo
as part of the Luma/Shield corpus split.

## Context

The system's earlier state (v2, per the same source's own retrospective)
allowed design freedom that was actively working against clarity:
navigation concepts leaked in, "one screen" wasn't absolute, and
imperative commands ("trigger," "send," "initiate") mixed freely with
newer state-based thinking. This was identified as a source of
ambiguity and drift, not a strength.

## Decision

**Interface model:**
- There is only one screen. No navigation, no menus, no back stacks.
- The user shifts *focus* between four things: Shield, Person, Packet,
  Context — they don't navigate between screens.

**Functional roles:**
- Shield = Action
- ~~Window = Context~~ — "Window" is superseded terminology (see
  [reconciliation/2026-09-07-core-not-pearl.md](../../reconciliation/2026-09-07-core-not-pearl.md)).
  The underlying idea (a display-only, non-action context layer)
  hasn't been re-stated under current naming — treat this half of the
  functional-role split as an open question, not settled.

**Constraint law:**
> One Tap or It Fails.

Every action must resolve in a single interaction. A multi-step
interaction is treated as a system failure, not a UX compromise to
optimize later.

**Language rule:** system behavior is described in state-based terms
only (`State Active`, `Packet Emitted`, `Packet Propagating`, `Routing
Active`). Imperative/command language (`Send`, `Trigger`, `Execute`,
`Initiate`) is prohibited — the system describes what *is happening*,
not what to do.

## Consequences

- Removes an entire class of UX complexity by construction — there's no
  "add one more menu" escape hatch.
- Raises the bar for every feature: if it can't resolve in one tap, per
  this doctrine it doesn't ship as designed, or it needs a doctrine
  exception logged as its own decision.
- Any engineering or design proposal that reintroduces multi-step flows
  or imperative-style APIs/copy is a doctrine violation, not a stylistic
  choice — should be caught at reconciliation, not shipped first.
