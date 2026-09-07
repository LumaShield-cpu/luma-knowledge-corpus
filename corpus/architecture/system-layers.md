# System layers

**Source:** [ARCH-02 — Translation Engine, Volume I, v1.0.0](../../sources/docs/arch-02-shield-labs-translation-engine-volume-i-v1.0.0.docx.meta.md),
§19. Approved by Stacey Malitowski, Project Owner, 2026-09-06.
**Supersedes:** the earlier CanonOS/DesignOS/ScreenOS/EngineeringOS
framing — see
[reconciliation/2026-09-07-volume-split-supersedes-canonos-layers.md](../../reconciliation/2026-09-07-volume-split-supersedes-canonos-layers.md).

Shield Labs is the governing organization. LumaShield is a
privacy-first coordination infrastructure product built on this
architecture. The constitutional structure is exactly two volumes:

| Volume | Name | Responsibility |
| --- | --- | --- |
| **Volume I** | Translation Engine | Evidence ingestion, operational-knowledge formation, validation, adjudication, governance, release, and Operational Context Package (OCP) formation. See [translation-engine.md](translation-engine.md). |
| **Volume II** | Enterprise SHIELD | Deterministic context resolution, experience composition, device-adaptive rendering, human resolution evidence, governed feedback. |

The two volumes interoperate through **typed, versioned,
policy-enforced contracts** — they are explicitly "not one
undifferentiated runtime." The shared contract between them is the
Operational Context Package (OCP): Volume I's output, Volume II's
input.

## Boundary discipline

Volume I **does not own**: live user-intent resolution, the Context
Resolution Engine, the runtime decision service, the Experience
Composition Engine, the Interaction Grammar, the Semantic Experience
Manifest, device capability negotiation, browser rendering, or Core /
Ring / Pads / Dial / Adaptive Operational Briefing behavior. All of
that is Volume II.

Volume I **does own**: source/evidence governance, translation and
atomization of evidence into candidate assertions, the Operational
Knowledge Graph, validation and adjudication, promotion/release, and
deterministic OCP assembly and delivery.

Neither volume may perform the other's job. Volume I "must not
precompute runtime decisions into operational truth"; Volume II must
treat Volume I's released knowledge as authoritative and cannot
originate it.

## Why this replaced the earlier framing

An earlier source (a pre-reset chat export, "Unified Canon State v3")
described four layers — CanonOS, DesignOS, ScreenOS, EngineeringOS —
plus a separate ingestion gatekeeper. That framing correctly identified
*that* truth-governance needed separating from rendering/presentation
concerns, but the actual approved architecture organizes that
separation differently: two volumes with a typed contract between them,
not four named "OS" layers. See the reconciliation record linked above.

## Status

This is the current, formally approved architecture as of 2026-09-06.
It is still a logical architecture — ARCH-02 is explicit that it "does
not declare any present implementation conformant." Whether a given
build actually implements this boundary is a separate, open question.
