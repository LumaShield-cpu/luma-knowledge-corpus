# Decision 0005: The artificial-intelligence boundary (Volume I)

**Status:** Locked — formally approved
**Source:** [ARCH-02 — Translation Engine, Volume I, v1.0.0](../../sources/docs/arch-02-shield-labs-translation-engine-volume-i-v1.0.0.docx.meta.md),
§11. Approved by Stacey Malitowski, Project Owner, 2026-09-06.

## Context

The Translation Engine is explicitly built to keep AI from
"manufacturing operational authority." This decision draws the line
between where AI helps and where it categorically cannot act, and
requires every approved AI use to be bound to specific, auditable
configuration rather than used loosely.

## Decision

**Permitted** (subject to source permission, data classification,
model approval, and output validation): OCR correction and
segmentation proposals; entity/relation extraction proposals;
classification and taxonomy mapping; ambiguity and conflict detection;
draft summaries and labels; candidate clause formation; cross-case
comparison; research evaluation and error analysis.

**Prohibited**, without exception: AI must not serve as evidence for
its own output; approve or release an assertion or OCP; resolve a
consequential policy decision; suppress conflicting evidence; modify
released knowledge directly; promote feedback/telemetry/an HRD into
operational truth; authorize access or delegation; execute
consequential write-back; select an unapproved model, prompt, tool,
connector, or data destination; or claim confidence as proof of
correctness or authority.

**Every approved model use must bind**, at minimum: provider and
service boundary; exact model and configuration version; approved
prompts/tools/output schema; allowed data classes and prohibited
content; retention and training terms; subprocessors and destination
jurisdictions; evaluation set and acceptance thresholds; abstention and
human-review rules; and per-run provenance, latency, and cost records.
"Bring Your Own LLM" does not authorize arbitrary models or
unrestricted data transfer.

## Consequences

- An AI assistant (including this one, working on this corpus) may
  propose candidate content, draft summaries, and flag conflicts — but
  writing something into `corpus/` as settled canon is a release
  decision, and per INV-09/this boundary, that authority belongs to an
  accountable human, not the model doing the drafting.
- This is a second, independent formalization of the lesson recorded in
  [reconciliation/2026-09-07-expression-engine-not-canon.md](../../reconciliation/2026-09-07-expression-engine-not-canon.md) —
  first learned by mistake in this corpus's own process, now confirmed
  as explicit product architecture.
