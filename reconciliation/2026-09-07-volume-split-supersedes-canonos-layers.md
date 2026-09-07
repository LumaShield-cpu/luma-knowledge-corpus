# Reconciliation: Volume I / Volume II supersedes the CanonOS/DesignOS/ScreenOS/EngineeringOS split

**Date:** 2026-09-07
**Author:** Stacey (via reconciliation session)

## Conflict

[corpus/architecture/system-layers.md](../corpus/architecture/system-layers.md)
was drafted from
[Unified Canon State v3](../sources/docs/lumacanonos-unified-canon-state-v3.md),
describing four layers — CanonOS, DesignOS, ScreenOS, EngineeringOS —
plus an ingestion pipeline gatekeeper.

[ARCH-02](../sources/docs/arch-02-shield-labs-translation-engine-volume-i-v1.0.0.docx.meta.md),
a formally approved architecture document (§19), instead defines
exactly two constitutional volumes:

| Volume | Name | Responsibility |
| --- | --- | --- |
| Volume I | Translation Engine | Evidence ingestion, operational modeling, candidate knowledge, validation, adjudication, governance, release, OCP formation |
| Volume II | Enterprise SHIELD | Deterministic context resolution, experience composition, device-adaptive rendering, human resolution evidence, governed feedback |

Neither "CanonOS," "DesignOS," nor "ScreenOS" appears anywhere in
ARCH-02. "Ingestion" survives, but as a responsibility *within* Volume
I (source and evidence governance), not as a separate fifth layer.

## Evidence

Per ARCH-02 §20.1's own source-authority hierarchy (see
[CONTRIBUTING.md](../CONTRIBUTING.md)), this document outranks the V3
chat export for Volume I architecture matters — V3 falls into the
hierarchy's lowest tier ("earlier diagrams, manuals, whiteboards,
generated syntheses... as non-authoritative evidence or design
history"). ARCH-02 is also dated 2026-09-06 with a recorded approval,
while V3 is an undated, informal chat export.

## Resolution

The CanonOS/DesignOS/ScreenOS/EngineeringOS framing is superseded. The
governing structure is the two-volume split (Translation Engine /
Enterprise SHIELD) as defined in ARCH-02 §19.

This is not necessarily a full repudiation of the *underlying idea* in
the old framing — separating truth-governance from
rendering/presentation concerns survives, just reorganized under
different names and a cleaner two-volume boundary rather than four
named "OS" layers. The V3 material remains useful evidence of *why*
that separation mattered (see the "why the separation exists" material
carried over into the corpus doc), just not of the resulting structure.

## Corpus update

[corpus/architecture/system-layers.md](../corpus/architecture/system-layers.md)
rewritten to describe the Volume I / Volume II split, citing ARCH-02.
