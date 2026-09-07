# Decision 0003: Ring and Glow — state as color, not decoration

**Status:** Locked (per source; not yet re-confirmed against current build)
**Source:** [Unified Canon State v3](../../sources/docs/lumacanonos-unified-canon-state-v3.md), §4.
**Corroboration:** the color set and the red/green prohibition both
appear independently in
[Luma Shield Documentation](../../sources/docs/luma-shield-documentation.md)
("Glow Culture colors are Teal, Amber, Violet. Red and green are
forbidden.") — an independent source agreeing on both the palette and
the exclusion strengthens this beyond a single-source claim.
**Structure confirmed and corrected 2026-09-07:**
[SHIELD Architecture Series, Volume III](../../sources/docs/shield-architecture-series-volume-iii.pdf.meta.md)
established that Ring and Glow are two distinct elements, not one — see
[reconciliation/2026-09-07-ring-and-glow-split-red-stays-forbidden.md](../../reconciliation/2026-09-07-ring-and-glow-split-red-stays-forbidden.md).
That same source also proposed adding Red as a real canon color; this
was checked and rejected — **Red and green remain forbidden.**

## Context

"Glow culture" is one of the system's standing principles: notifications
are replaced by ambient color/light state rather than text alerts or
badges. Before v3, glow existed visually but not "linguistically" — colors
were chosen but timing, persistence, and meaning weren't formally
defined, so the same color could be read inconsistently.

## Decision

**Color canon** (exhaustive — no other colors are canon; this applies
across both Ring and Glow, described below):

| Color | Meaning |
| --- | --- |
| White | Idle / off |
| Teal | Presence / connection active |
| Amber | Attention / context signal |
| Violet | Action / response active |

**Red and green are explicitly forbidden** — this is a deliberate
departure from conventional status-color conventions (success=green,
danger=red), consistent with the doctrine of calm, non-alarming
interaction (no panic UI, no alarms). This was directly re-checked
against a competing draft proposal to introduce Red and reaffirmed —
see the reconciliation record above.

**Scope note (2026-09-07):** this ban applies to the broader Shield
(professional/business) architecture. LumaShield's own,
separately-scoped design system
([shield-canon](https://github.com/Solid-Stride/shield-canon), a
separate repo — out of this corpus's scope, see the reconciliation
record below) is confirmed exempt — it uses red for `danger`/`error` tokens as its own
product-level choice, the same precedent as the
[four-Pad layout](../architecture/shield-anatomy.md). See
[reconciliation/2026-09-07-shield-canon-collision.md](../../reconciliation/2026-09-07-shield-canon-collision.md).
Don't read this exemption as loosening the rule anywhere else.

### Ring — discrete operational state

The Ring communicates **discrete** state: connected, in progress,
blocked, waiting. It's always visible when a Shield is active; the
*absence* of an active expression is itself a state (settled, calm,
functioning normally). A user should be able to perceive Ring state
without actively reading or querying it.

**Layers:** Core Glow, Pad Glow, Shield Glow, Device Glow — state can
be expressed at different structural levels, not just one indicator
light.

**Output surfaces:** Halo (preferred), full screen (limited use), Shield
shape (lock screen / wearable).

### Glow — ambient, continuous character layer

Glow is a separate, continuous layer expressing the **ambient felt
quality** of the current moment (calm, active, watchful, resolved) —
distinct from Ring's discrete state signals. It operates at the
periphery of attention: perceptible without demanding focus,
meaningful without decoding.

**Behavior types:**
- Nudge — single slow pulse
- Waiting — continuous pulse
- Emotional / acknowledgment — slow, continuous rhythm

Glow must remain calm under all circumstances — no strobing, no rapid
alternation, nothing that reads as alarm or panic, even in
high-consequence moments. The system communicates urgency without
communicating panic.

**Status note:** Volume III's specific named Glow states (Calm
Presence, Active Coordination, Watch State, Action Required, Concern,
Completion) are plausible draft-tier illustrative detail, not
independently re-verified — treat as examples, not confirmed canon,
until reconciled on their own.

## Consequences

- Any feature proposing red or green as a status color is a doctrine
  violation, not a design preference — this should be caught early,
  including in visual QA, not just in canon review. This has now been
  checked twice (original sourcing, and against a later draft that
  proposed adding Red) and confirmed both times.
- Ring and Glow are separate design surfaces — a feature that only
  updates one when it should update both (e.g., a state change that's
  discrete but doesn't touch the ambient character layer, or vice
  versa) may be incomplete, not just a stylistic choice.
- New states must be expressed by combining existing colors, behavior
  types, and layers — not by introducing a fifth color, which would be
  a canon change requiring its own decision record.
