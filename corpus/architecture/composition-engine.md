# Composition Engine (engineering detail)

**Source:** [SHIELD Architecture Series, Volume II — Part II: Composition Architecture](../../sources/docs/shield-architecture-series-volume-ii-part-ii.pdf.meta.md).
Self-marked "Current Working Framework v0.2 · Not Final Canon ·
Technical Architecture Draft."

**Status: draft-tier detail, not approved canon** — same caveat as
[translation-pipeline.md](translation-pipeline.md). This document
predates the Core/AOB naming correction and uses "Pearl" and "Context
Window" throughout; per
[reconciliation/2026-09-07-core-not-pearl.md](../../reconciliation/2026-09-07-core-not-pearl.md),
this corpus doc uses **Core** wherever the source says "Pearl." No
other conflicts found — the underlying pipeline and governance content
is consistent with [enterprise-shield.md](enterprise-shield.md) and
ARCH-02's invariants.

## What it does

The Composition Engine turns a validated OCP (Translation Engine's
output) into an **Adaptive Operational Workspace** — the concrete
answer to "what should this human experience right now," resolved
fresh at runtime rather than pre-designed. Its own framing: *"The
Translation Engine understands the operational world. The Composition
Engine brings that understanding to the human."*

## The resolution pipeline

**Identity Resolve → Intent Resolve → Context Resolve → Permission
Resolve → Capability Select → Experience Compose.** Stages don't merge
— each is independently auditable, replaceable, and testable.

- **Identity Resolution** — a person may hold multiple concurrent
  identities (Personal, Professional, Organizational, Temporary,
  Event-based, Role-based...); resolution determines which is active
  without conflating them.
- **Intent Resolution** — explicit or inferred from signals
  (location, time, calendar, active task, sensor state). *"SHIELD is
  context-first, not prompt-first"* — it shouldn't ask what it can
  already infer.
- **Context Resolution** — synthesizes identity + role + intent with
  environmental signals into what matters right now. Canonical law:
  *"Context precedes interaction."*
- **Permission Resolution** — dynamic, evaluated at runtime against
  identity/role/context/relationship/policy/time — not a static ACL.
  Explicitly: *"AI-generated suggestions do not automatically become
  valid capabilities. Every composed capability must pass Permission
  Resolution before surfacing."*
- **Capability Selection** — chooses which operational abilities
  (inspect, approve, pay, escalate, etc.) are relevant *and* permitted
  right now — not every feature the system could show.
- **Experience Composition** — assembles the actual workspace: what's
  in the workspace, which Pads are active, what the Core confirms, what
  the Ring communicates. No layout is pre-designed.

## The Composition Artifact Package

Every run produces a structured package (paralleling the Translation
Engine's own artifact package): current operational context, identity
and intent resolution records, permission map, capability selection
map, the Adaptive Workspace Specification, the Shield Runtime
Specification (Dial/Pad/Core/Ring configuration), device rendering
spec, active Nudge/Beacon rules, expert-escalation rules, a memory
update recommendation (pending governance approval), a per-dimension
confidence report, an integrity validation report, and an audit
record.

## Device rendering — one grammar, adaptive surfaces

The interaction grammar (Shield/Dial/Pads/Core/Ring) never changes
across devices; only the rendering does. Named modes: **Phone**
(highest-constraint, one-tap, voice-first), **Foldable** (larger
context area, persistent Dial, dual-context display), **Tablet**
(multiple context frames, sustained engagement), **Desktop** ("not a
separate product — a richer rendering of the same operational
context"), **Watch** (ambient-only: Ring state + one actionable prompt,
not an action surface), **Vehicle** (voice-first, zero visual density,
maximum cognitive-safety constraints), **AR** (spatial overlays —
composed only when contextually appropriate, not just because hardware
supports it). One Composition Engine; the Device Rendering
Specification carries the per-surface parameters, so new surfaces
extend the contract rather than forking the composition logic.

## Runtime state and the connection lifecycle

**Foundational privacy guarantee:** *"A Shield connection begins. A
Shield connection ends. Privacy returns... There is no state from
which privacy cannot be restored."* Every adopted or shared context has
a defined path back to a private state; this is enforced structurally
by the runtime state machine, not left as a convention.

Three distinct, non-interchangeable levels of engaging a Shield:
- **Reveal** — preview scope/capabilities/governance terms; no data
  shared, no permission required.
- **Adopt** — temporarily activate a Shield context; live, governed,
  revocable; requires permission.
- **Ingest** — import a governed operational asset permanently into
  your own environment, with its own governance record.

## Coordination primitives: Nudge and Beacon

- **Nudge** — a low-friction prompt (confirm, acknowledge, review) —
  explicitly not a notification or alert; must not fire during an
  active protocol or high-urgency moment unless safety-relevant.
- **Beacon** — a formal, scoped request for organizational/network
  help when existing knowledge can't resolve something — carries
  problem statement, constraints, urgency, permission scope, and an
  expiration. Composed by the engine from context, not manually typed.

## Expert escalation ("Ask [Expert]") and the Operational Ambassador

A generalized escalation pattern, not a specific named agent: use
existing knowledge first → escalate to a known expert if insufficient →
capture the expert's response as a **Decision Object** (decision,
reason, alternatives, actor, context, evidence, date, impact,
review status) → update operational memory on approval.

The AI's role is explicitly framed as an **"operational
ambassador," not a chatbot** — and not the expert: *"the AI does not
pretend to be the expert."* It carries context, reduces interruption,
drafts requests, and preserves decisions, but acts only on the user's
behalf, never generating commitments without confirmation. This
extends [decision 0005's AI boundary](../decisions/0005-ai-boundary.md)
with concrete permitted/prohibited lists:

- **AI may:** interpret intent, summarize context, recommend layout,
  draft escalations, retrieve memory, ask clarifying questions.
- **AI may not:** own the context model, override permissions, bypass
  validation, determine governance, represent itself as a domain
  expert, or generate commitments without confirmation.

Also stated as an explicit architectural requirement: the platform must
stay **model-agnostic and cloud-portable** — no foundation-model
provider may become a structural dependency.

## Safety: confidence and fallback

Eight independently-scored confidence dimensions (identity, intent,
context, permission, capability, layout, risk, recommendation). If any
falls below threshold, the engine degrades to a safe fallback (ask a
clarifying question, show read-only context, require human approval,
offline/emergency mode, return to private state) rather than proceed
uncertainly. Stated as an absolute: *"uncertain composition must never
produce unsafe action."*

## Shield composition patterns (worked examples)

The same OCP, composed differently by role/context — not different
products: **Professional Shield** (a professional's client queue vs.
a client's service status — "same operational asset, different
composition, the professional is amplified, not replaced"),
**Service Shield** (HVAC/home-service dispatch with full context
attached), **HomeShield** (a home as one composed operational
environment, not just a contacts list), **Academic Shield**
(Student/Professor/Research Shield as three role-compositions of one
institutional context), **Organization Shield** (modular capability
Shields — Accounting, Safety, Fleet, HR... — composed, not a suite of
separate apps).

## Status

Consistent with, and a detailed elaboration beneath,
[enterprise-shield.md](enterprise-shield.md) — no conflicts found
beyond the already-reconciled Pearl/Core naming. Treat as
well-corroborated draft-tier detail, not locked canon.
