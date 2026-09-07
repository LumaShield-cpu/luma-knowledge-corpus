# Decision 0004: The twelve constitutional invariants (Volume I)

**Status:** Locked — formally approved
**Source:** [ARCH-02 — Translation Engine, Volume I, v1.0.0](../../sources/docs/arch-02-shield-labs-translation-engine-volume-i-v1.0.0.docx.meta.md),
§4. Approved by Stacey Malitowski, Project Owner, 2026-09-06.

## Context

Before this canonization, multiple informal sources (chat exports,
drafts) made confident-sounding claims about how evidence becomes
"truth" in the system, without a settled, binding standard for what
counts as evidence, who may approve what, or how conflicts and
uncertainty get handled. ARCH-02 fixes this with twelve invariants that
"all conforming Volume I designs and implementations SHALL preserve."

## Decision

| ID | Invariant |
| --- | --- |
| INV-01 | Evidence precedes assertion. Non-synthetic claims must resolve to registered sources; synthetic/inferred/model content must be labeled, never passed off as evidence. |
| INV-02 | Candidate is not authoritative. Extraction, model output, feedback, telemetry, and imports all enter as candidate material unless an approved rule and release authority say otherwise. |
| INV-03 | Authority, confidence, freshness, and access are independent. They must not be collapsed into one score — high confidence does not create authority. |
| INV-04 | Conflicts remain representable. The engine must never silently average, merge, overwrite, or conceal conflicting assertions. |
| INV-05 | Absence is not negative evidence. Missing or unsearched evidence stays visible in corpus accounting — it isn't auto-interpreted as proof a condition is false. |
| INV-06 | No bypass. Structured ingestion may skip AI, but never schema validation, provenance, policy, conflict handling, required human authority, or release governance. |
| INV-07 | Immutable released history. Released assertions and OCP versions are never overwritten — only superseded, revoked, or rolled back via a new governed release. |
| INV-08 | Operational meaning is presentation-independent. An OCP must never contain device layouts, pixel coordinates, or a mandated UI implementation. |
| INV-09 | AI has no release authority. No model may approve, release, revoke, or operationalize knowledge, authorize access, or perform consequential write-back. |
| INV-10 | Deterministic governed handoff. An OCP delivered to Enterprise SHIELD must be assembled from explicitly versioned, released inputs under reproducible selection rules. |
| INV-11 | Tenant and purpose boundaries are enforced at policy/data-access points — a tenant ID as an ordinary field is not isolation. |
| INV-12 | Research does not self-authorize production. Finishing a prototype or Phase 1 deliverable never on its own authorizes production deployment or Volume II construction. |

## Consequences

- Any proposed feature, schema, or process that would let a model's
  output become "released" knowledge without going through validation
  and an accountable approval step violates INV-02/INV-09 outright —
  this should be caught in review, not shipped and corrected later.
- Any design that "resolves" a conflict by picking one side and
  discarding the other (rather than preserving both, adjudicated)
  violates INV-04.
- This directly reinforces a lesson this corpus already learned the
  hard way (see
  [reconciliation/2026-09-07-expression-engine-not-canon.md](../../reconciliation/2026-09-07-expression-engine-not-canon.md)):
  INV-02 and INV-09 formalize, at the product-architecture level, the
  same principle CONTRIBUTING.md's source-authority section applies to
  this corpus's own process — AI output is candidate material, not
  truth, until something accountable ratifies it.
