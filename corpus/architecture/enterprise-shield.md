# Enterprise SHIELD (Volume II)

**Sources:** [ARCH-02](../../sources/docs/arch-02-shield-labs-translation-engine-volume-i-v1.0.0.docx.meta.md)
§19 (naming and constitutional boundary); [shield-edge.pdf](../../sources/docs/shield-edge.pdf.meta.md)
(architecture detail, superseding the earlier "plain SHIELD" naming —
see [reconciliation/2026-09-07-shield-edge-naming-and-deployment.md](../../reconciliation/2026-09-07-shield-edge-naming-and-deployment.md)).

See [composition-engine.md](composition-engine.md) for the
engineering-level resolution pipeline (Identity → Intent → Context →
Permission → Capability → Experience) beneath this description —
draft-tier, but consistent with everything below.

## What it is

Volume II — **Enterprise SHIELD** ("Semantic Human Intelligence &
Execution Layer Domain") — is the deterministic context-resolution,
experience-composition, and rendering half of the Shield Labs
architecture, paired with [Volume I / the Translation Engine](translation-engine.md).
Where Volume I answers "what is operationally true," Enterprise SHIELD
answers "what should this human see and do right now" — and renders
it, without ever originating operational truth itself.

Its own canonical declaration: it "discovers nothing and invents
nothing. It transforms." Volume I discovers operational truth; the OCP
preserves it; Enterprise SHIELD transforms that truth into deterministic
human experience.

## Deployment forms — Shield, Enterprise SHIELD, and SHIELD Edge

These are three different ways this architecture reaches a human, not
three different architectures:

- **Shield** and **Enterprise SHIELD** (as products) — **installed**,
  native clients.
- **SHIELD Edge** — the **browser-based, on-device rendering kernel**:
  no proprietary client, standards-based, deployable across connected,
  offline, and air-gapped environments with an identical pipeline and
  governance model in all three. This is a way of *realizing* the same
  architecture without installation, not a separate fourth system.

## The six rendering layers

1. **Verified Operational Context** — final schema/provenance/policy
   validation of an incoming OCP.
2. **Context Resolution Engine (CRE)** — resolves identity, location,
   device, task, urgency into a **Resolved Experience State**.
3. **Experience Composition Engine (ECE)** — the architectural heart.
   Deterministically resolves (never generates) a **Semantic Experience
   Manifest** against a governance-authored **Composition Rule
   Graph** — AI may help author that graph offline, but plays no role
   in runtime composition.
4. **Semantic Experience Manifest** — a device-independent declaration
   of what must be experienced (regions, priority, evidence, motion
   permissions), never pixels or layout.
5. **Universal (Browser) Rendering Kernel** — physically renders the
   manifest on-device; this is the layer SHIELD Edge specifically names.
6. **Governed Interaction Capture** — every interaction returns to
   Volume I as candidate evidence, never as self-promoted truth.

## Interaction primitives

Five semantic primitives, confirmed consistently across `shield-edge.pdf`
and [ARC-01's terminology dictionary](../../sources/docs/arc-01-shield-canonical-terminology-and-relational-architecture-v0.1.docx.meta.md)
(no live use of "quadrant" anywhere in either):

- **Core** — the single highest-priority focal element for the current
  moment; exactly one per composed experience; resolved by the ECE,
  never user-chosen.
- **Pads** — grouped contextual regions (situation, evidence,
  personnel, resource, decision, timeline); derived by the ECE, not
  fixed screens.
- **Ring** — the persistent, ambient, non-interruptive awareness layer.
- **Dial** — a governed lens for changing depth/time/scope without
  altering underlying authority; replaces menu navigation.
- **Adaptive Operational Briefing (AOB)** — the composite envelope
  binding Core + Ring + Pads + Dial for one operational moment.

**Note:** ARC-01 (a not-yet-approved proposal) marks Core and AOB as
"Adopt with correction" and Ring/Pads/Dial as "Adopt as provisional
primitive" — meaning even the primitives themselves aren't fully
locked yet, just converged-upon in every source checked so far.

## Governing invariant

Enterprise SHIELD must never precompute Volume I's job into operational
truth, and Volume I must never perform Enterprise SHIELD's runtime
resolution, composition, or rendering. Human judgment remains
authoritative throughout — SHIELD surfaces decisions, it doesn't make
them.

## Status

Architecturally described in detail across multiple sources with
strong internal agreement (see above), but **not itself the subject of
a formal, hash-bound approval instrument** the way ARCH-02 (Volume I)
and the Volume II v0.2 monograph addendum are. Treat this doc as
well-corroborated design description, one tier below constitutional
canon, pending an equivalent approved instrument for Volume II as a
whole.

A much larger, actively-developing source exists —
[shield-edge-architecture-canonical-consolidated-export-2026-09-06.md](../../sources/docs/shield-edge-architecture-canonical-consolidated-export-2026-09-06.md),
covering through section 12,233 of an ongoing canon — introducing
further subsystems (IADR, SCK, AMC, HRD) not yet reconciled into this
doc. That's the natural next source to work through.
