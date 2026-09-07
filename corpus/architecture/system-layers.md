# System layers

**Source:** [Unified Canon State v3](../../sources/docs/lumacanonos-unified-canon-state-v3.md), §1 and §11.

LumaShield is a **human coordination protocol platform** — not "an app,"
but a state-based coordination language expressed through visual
interfaces called Shields (see [expression-engine.md](../decisions/0002-expression-engine.md)).

## Layers

| Layer | Role |
| --- | --- |
| **CanonOS** | Source of truth. Governs definitions and rules for every other layer. |
| **DesignOS** | Enforces visual and interaction rules (see [interaction-doctrine.md](../decisions/0001-interaction-doctrine.md), [glow-system.md](../decisions/0003-glow-system.md)). |
| **ScreenOS** | Rendering logic. |
| **EngineeringOS** | Implementation layer. As of the v3 snapshot, not yet canonized in structure — it consumes canon rather than defining it. |
| **Ingestion pipeline** | Gatekeeper between new input and Canon. Nothing becomes canon by bypassing it. |

## Why the separation exists

Before this separation was enforced, canon, design, and engineering
concerns overlapped freely — design changes could redefine structure,
engineering assumptions could leak into canon, and multiple sources
could claim to define "truth" at once. The v3 source describes this
directly as the prior (pre-lock) state:

> Canon, Design, and Engineering were overlapping. Ingestion not fully
> policing. Multiple sources influencing "truth." Canon was still
> negotiable.

Separating the layers, with CanonOS as the sole authority and ingestion
as a gate, was the fix: no layer should define truth for another, and
nothing enters canon without passing through ingestion.

## Status

This is an architectural intent captured in a single (pre-reset) source
and not yet independently re-confirmed against current engineering
reality. Treat the layer *names and responsibilities* as canon; treat
"is this actually enforced in the current build" as an open question
for a future reconciliation pass once engineering sources are pulled
into this corpus.
