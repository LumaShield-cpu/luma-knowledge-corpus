# Translation Engine (Volume I)

**Source:** [ARCH-02 — Translation Engine, Volume I, v1.0.0](../../sources/docs/arch-02-shield-labs-translation-engine-volume-i-v1.0.0.docx.meta.md).
Approved by Stacey Malitowski, Project Owner, 2026-09-06 ("Agreed.
Proceed."). Status per document: **Canonical Architecture —
Implementation Conformance Pending** — the architecture is approved;
no implementation is yet certified to conform to it.

## What it is

> The Translation Engine is Shield Labs Volume I. Its constitutional
> responsibility is to transform permitted source evidence into
> governed, versioned, provenance-preserving operational knowledge
> that can be consumed safely by Enterprise SHIELD, without allowing
> extraction systems, analytical systems, or artificial intelligence to
> manufacture operational authority.

The canonical spine: **Approved sources → Immutable evidence records →
Translation and atomization → Candidate assertions → Validation and
adjudication → Released operational knowledge → Deterministic OCP
assembly → Governed handoff to Enterprise SHIELD.** No stage may be
bypassed.

## Logical domains

Seven domains, each with a defined input, output, and mandatory failure
behavior: Research and Model Governance; Source and Evidence;
Translation and Atomization; Operational Knowledge; Validation and
Adjudication; Promotion and Release; OCP Assembly and Delivery. Every
domain fails closed — e.g. Promotion and Release "fails closed on
missing approval, policy, version, or release evidence" rather than
defaulting to permissive behavior.

## Knowledge lifecycle

Every candidate or released assertion moves through a fixed state
machine: **Candidate → Under Review → Validated → Approved → Effective
→ (Superseded | Revoked)**, or **Rejected** if review fails. Every
transition produces an immutable record — no transition may be
inferred from a bare field mutation.

Key distinctions the lifecycle enforces:
- **Validated is not Approved.** Passing checks doesn't grant release
  authority.
- **Effective, Superseded, and Revoked all preserve history.**
  Corrections happen through new versions, not overwrites (see
  invariant INV-07 below).

## The Operational Context Package (OCP)

The OCP is the sole handoff artifact from Volume I to Volume II. It
must be assembled deterministically from released, version-bound
assertions; declare its scope/tenant/jurisdiction/effective
interval/profile; preserve provenance and unresolved
conflicts/uncertainty; and remain **independent of any specific
screen, device, or presentation framework**. It fails validation
outright if required fields, evidence, versions, or authorities are
missing — there is no silent degraded mode.

**Status note:** the "OCP Profile 0.1" (a proposed 16-section payload
structure) is explicitly a research artifact, not the production
standard. No other packet family inherits its section structure.

## Constitutional invariants and the AI boundary

See [0004-constitutional-invariants.md](../decisions/0004-constitutional-invariants.md)
and [0005-ai-boundary.md](../decisions/0005-ai-boundary.md) for the
twelve binding invariants and the specific rules governing what AI may
and may not do within this architecture.

## Explicitly rejected interpretations

ARCH-02 §18 lists interpretations incompatible with it, including:
all packets sharing one exact 16-section payload; a 4×4×4 or 16×4
pattern being "a proven universal law" (a packet/schema-level claim —
see
[reconciliation/2026-09-07-four-pads-vs-rejected-numerology.md](../../reconciliation/2026-09-07-four-pads-vs-rejected-numerology.md)
for why this doesn't touch the Shield's 4-Pad interface anatomy); model
output being evidence or released truth; confidence creating authority;
and the architecture "guaranteeing zero semantic drift, perfect
accuracy, or complete safety."

## Source authority (as ARCH-02 itself defines it)

ARCH-02 §20.1 ranks, for Volume I matters, in order: (1) explicit
project-owner approval and subsequent approved decisions; (2) ARCH-02
itself; (3) the High-Level Architecture Companion, where non-conflicting;
(4) the Translation Engine Master Reference, as a Phase 1 research
annex, where non-conflicting; (5) approved downstream schemas/specs/ADRs
within delegated scope; (6) **everything else — earlier diagrams,
manuals, whiteboards, generated syntheses, domain scenarios — as
non-authoritative evidence or design history.**

Almost everything else currently in `sources/docs/` (the ChatGPT
exports, the V3 snapshot, the draft SHIELD Architecture Series volumes)
falls into tier 6 for any Volume I question. This doesn't make that
material worthless — it's design history and may be the only evidence
available for something ARCH-02 doesn't cover — but it means ARCH-02
wins on conflict, not the other way around.
