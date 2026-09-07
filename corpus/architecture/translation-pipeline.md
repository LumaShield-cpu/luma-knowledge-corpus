# Translation pipeline (engineering detail)

**Source:** [SHIELD Architecture Series, Volume II — Part I: Translation Architecture](../../sources/docs/shield-architecture-series-volume-ii-part-i.pdf.meta.md).
Self-marked "Current Working Framework v0.2 · Not Final Canon ·
Technical Architecture Draft."

**Status: draft-tier detail, not approved canon.** Unlike
[translation-engine.md](translation-engine.md) (drawn from ARCH-02,
constitutional canon), this document elaborates the same Volume I
system at engineering granularity without itself carrying formal
approval. Everything below is consistent with, and fills in detail
beneath, ARCH-02's invariants and lifecycle — no conflicts found. Treat
this as well-corroborated design detail, not a locked decision.

## The pipeline

**Ingestion → Knowledge Corpus → Extraction → Operational Knowledge
Model (OKM) → Operational Knowledge Graph (OKG) → Operational Context
Model (OCM) → Operational Context Package (OCP) → Shield Integrity
Layer (SIL) → handoff to the Composition Engine.**

- **Ingestion** reads/normalizes/classifies artifacts without
  interpreting them — a fidelity-preservation stage only. Every
  artifact gets a source ID, fingerprint, provenance record, and
  classification before it can proceed.
- **Knowledge Corpus** is the append-only, preserved source-of-truth
  collection — "organized evidence," not yet intelligence. If a later
  extraction is wrong, the Corpus itself stays untouched and can be
  reprocessed.
- **Extraction** converts artifacts into operational meaning, not
  layout: "a button is not a button — it is an Operational Event
  trigger." Every extracted entity normalizes to one of a fixed set of
  **core object types**: Organization/Person/Role, Asset/Location,
  Event/Task/Workflow/Protocol, Decision/Rule/State,
  Evidence/Connector/Destination, and Knowledge/Wisdom/Memory Package.
- **OKM** — the normalized, source-independent representation of what
  the organization does. Must express meaning, not the originating
  form's structure.
- **OKG** — the semantic graph connecting every OKM object to every
  other; what makes relationships computable and queryable.
- **OCM** — a *runtime-computed* overlay on the OKG answering "given
  who's acting, what they intend, and their state — what matters right
  now?" The Translation Engine defines it; the Composition Engine
  evaluates it live.
- **OCP** — the deployable handoff object: context identity,
  roles/permissions, entities/events, rules, evidence requirements,
  state model, connector recipes, destinations, knowledge references,
  and a confidence score. This is the same OCP [translation-engine.md](translation-engine.md)
  describes at the constitutional level, here given a concrete field
  list.

## Governance gates along the way

- **Shield Integrity Layer (SIL)** — mandatory; nothing reaches the
  Composition Engine without clearing policy/schema, permission/safety,
  and connector/audit checks. Canonical law: *"SHIELD may connect to
  anything, but nothing connected to SHIELD may violate SHIELD law."*
  Failures are quarantined, not silently dropped.
- **Translation Confidence** is scored per source type (schema-defined
  sources ~95%, structured artifacts ~80%, unstructured documents
  ~65%, human knowledge ~50%) and tracked across eight dimensions
  (source, extraction, semantic, connector, rule, context, safety,
  human-validation confidence). High-risk contexts cannot deploy on
  low-confidence translation without explicit human sign-off.
- **Validation Engine** — the explicit statement that "AI suggestion
  does not equal SHIELD capability": no AI-extracted output becomes an
  operational asset without passing schema, source, permission,
  security, and human-expert validation. This is the same principle as
  [decision 0004's INV-02/INV-09](../decisions/0004-constitutional-invariants.md)
  and [0005's AI boundary](../decisions/0005-ai-boundary.md), confirmed
  independently at the engineering-detail level.
- **Security/secret handling** — credentials are never allowed to
  remain in an operational definition; they're extracted to a governed
  secret vault and replaced with a reference, with an automatic
  security alert.
- **Versioning and provenance** — every object traces back through
  source artifact → translation record → human review → validation
  history → change history, with rollback to any prior validated
  state.

## Engineering breakdown (ENG-001 through ENG-009)

Nine discrete work packages: Corpus Ingestion Engine, Operational
Knowledge Extractor, OKG Generator, OCP Generator, Translation
Validation Engine, Connector Intelligence Extractor, Provenance and
Versioning Layer, Security and Secret Detection, and the Translation
Package Exporter (which assembles a standard 15-artifact Translation
Artifact Package for every run). Each has a defined purpose,
inputs/outputs, and acceptance criteria in the source document.

## The Translation/Composition boundary

Stated as a hard rule, worth repeating verbatim: *"Translation Engine:
operational understanding. Composition Engine: operational experience.
These are not the same thing and must not be designed as if they
are."* The Translation Engine's job ends at a validated,
SIL-cleared OCP — everything after that (adaptive workspace generation,
runtime context evaluation, human interaction) belongs to
[Enterprise SHIELD](enterprise-shield.md).
