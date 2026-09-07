# Decision 0003: The glow system — color as state, not decoration

**Status:** Locked (per source; not yet re-confirmed against current build)
**Source:** [Unified Canon State v3](../../sources/docs/lumacanonos-unified-canon-state-v3.md), §4.
**Corroboration:** the color set and the red/green prohibition both
appear independently in
[Luma Shield Documentation](../../sources/docs/luma-shield-documentation.md)
("Glow Culture colors are Teal, Amber, Violet. Red and green are
forbidden.") — an independent source agreeing on both the palette and
the exclusion strengthens this beyond a single-source claim.

## Context

"Glow culture" is one of the system's standing principles: notifications
are replaced by ambient color/light state rather than text alerts or
badges. Before v3, glow existed visually but not "linguistically" — colors
were chosen but timing, persistence, and meaning weren't formally
defined, so the same color could be read inconsistently.

## Decision

**Color canon** (exhaustive — no other colors are canon):

| Color | Meaning |
| --- | --- |
| White | Idle / off |
| Teal | Presence / connection active |
| Amber | Attention / context signal |
| Violet | Action / response active |

**Red and green are explicitly forbidden** — this is a deliberate
departure from conventional status-color conventions (success=green,
danger=red), consistent with the doctrine of calm, non-alarming
interaction (no panic UI, no alarms).

**Behavior types:**
- Nudge — single slow pulse
- Waiting — continuous pulse
- Emotional / acknowledgment — slow, continuous rhythm

**Layers:** Core Glow, Pad Glow, Shield Glow, Device Glow — glow state
can be expressed at different structural levels, not just one indicator
light.

**Output surfaces:** Halo (preferred), full screen (limited use), Shield
shape (lock screen / wearable).

## Consequences

- Any feature proposing red or green as a status color is a doctrine
  violation, not a design preference — this should be caught early,
  including in visual QA, not just in canon review.
- New states must be expressed by combining existing colors, behavior
  types, and layers — not by introducing a fifth color, which would be
  a canon change requiring its own decision record.
