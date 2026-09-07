<!--
Provenance
  Original title: ARC-01 -- SHIELD Canonical Terminology and Relational
  Architecture (Controlled Architecture Proposal and Volume I
  Integration Specification)
  Type: Word document (.docx) -- formal architecture proposal
  Version: 0.1
  Status (per document): Joint Review Draft -- Not Yet Effective
  Issue date: 2026-08-14
  Parent authority: Translation Engine Volume I v1.0 (see
  arch-02-shield-labs-translation-engine-volume-i-v1.0.0.docx.meta.md)
  Prepared for: Dr. Sidney Shapiro, Stacey Malitowski, Noel Roemmele
  Legal partner: Rugged Mobile Solutions Inc.
  Dropped locally: 2026-09-07, by stacey@solidstride.ca

  Status note: this document is explicitly NOT YET APPROVED ("Joint
  Review Draft... Approval requires a recorded joint disposition") --
  it sits below ARCH-02 in authority, as a proposal built on top of
  it, not itself canon. Its own abstract states it corrects prior
  overreach: it "replaces an asserted universal 16-section packet
  symmetry" and "recasts the claimed 64-node mathematical Lock as a
  16-by-4 coverage matrix" -- both consistent with claims rejected
  outright in ARCH-02 section 18. Contains a "Corrected Canonical Data
  Dictionary" (Core/Ring/Pads/Dial/AOB) that agrees with the SHIELD PDF
  already in this corpus and confirms no live use of "quadrant."
  Unreconciled against corpus/ -- see /CONTRIBUTING.md.
-->

# Extracted text (for reference -- verify against the original .docx before citing precisely)

Extracted via XML parsing (no pandoc/LibreOffice available in the
ingestion environment). Table rows are marked "[row end]"; formatting
and exact table structure (this is a long, heavily tabular document)
are not preserved -- verify precise field definitions against the
original before citing.

---





TRANSLATION ENGINE PROGRAM  •  ARCHITECTURE CONTROL SERIES
ARC-01
SHIELD Canonical Terminology
and Relational Architecture
Controlled Architecture Proposal and Volume I Integration Specification

Status: Joint Review Draft — Not Yet Effective
Version: 0.1
Issue date: 14 August 2026
Program period: 1 September–31 December 2026
Parent authority: Translation Engine Volume I v1.0
Prepared for: Dr. Sidney Shapiro • Stacey Malitowski • Noel Roemmele
Legal partner: Rugged Mobile Solutions Inc.
CONTROL DECISION
ARC-01 proposes a governed terminology and future runtime architecture. It does not amend Volume I, authorize production implementation, or convert hypotheses into validated findings.
Project-controlled. No client data included. Approval requires a recorded joint disposition.

Abstract
This controlled architecture proposal reconstructs the post-review Translation Engine and SHIELD terminology into an academically defensible, implementation-aware specification. It preserves Translation Engine Volume I as the governing four-month research foundation and assigns production architecture to a future Volume II. The proposal replaces an asserted universal 16-section packet symmetry with a Common Governed Envelope and typed OCP, IDP, IGP, HRD, observation, analytical, and manifest payloads. It defines IADR as a deterministic Permit / Deny / Abstain decision model, recasts the claimed 64-node mathematical Lock as a 16-by-4 coverage matrix, corrects the runtime sequence, and establishes knowledge-promotion, AI allow-list, identity, privacy, security, lifecycle, accessibility, performance, and test obligations. The result is suitable for joint concept review and bounded schema prototyping, but it is not a production system specification, cryptographic assurance claim, or evidence that the proposed architecture will succeed.
Keywords: Translation Engine; SHIELD; IADR; operational context; provenance; attribute-based access control; human resolution; responsible AI; architecture governance; experience composition
Controlled status. Terms become canonical only after recorded approval. Numeric targets, platform choices, cryptographic profiles, identity sources, and AI configurations remain proposed or open where evidence is incomplete.


Contents
Chapters and controlled appendices. Page references correspond to this rendered edition.  [row end]

Section
Page  [row end]

1  Executive Decision and Controlled Status
4  [row end]

2  Document Control and Use
7  [row end]

3  Research-to-Runtime Boundary
9  [row end]

4  Architecture Principles and Invariants
11  [row end]

5  Corrected Canonical Data Dictionary
13  [row end]

6  Layered Architecture and Volume Crosswalk
16  [row end]

7  Common Governed Envelope and Lifecycle
18  [row end]

8  Typed Packet Specifications
21  [row end]

9  IADR Decision Model
25  [row end]

10  Corrected Runtime Relational Sequence
28  [row end]

11  AI-Assisted Translation and Knowledge Promotion
30  [row end]

12  Security, Privacy, Legal, and Identity Assumptions
32  [row end]

13  Non-Functional Requirements and Verification
35  [row end]

14  Conformance and Test Strategy
37  [row end]

15  Open Questions and Decisions Required
39  [row end]

16  Change Impact and Implementation Roadmap
40  [row end]

17  Approval, Acceptance, and Review Record
42  [row end]

Appendix A — Common Governed Envelope Field Dictionary
44  [row end]

Appendix B — Supplied Proposition Disposition Crosswalk
48  [row end]

Appendix C — Worked Field Scenario
50  [row end]

Appendix D — ARC-01 Conformance Checklist
52  [row end]

Appendix E — Binder Amendment and Cross-Reference Instructions
54  [row end]

References
55


1  Executive Decision and Controlled Status
Decision requested
This document submits ARC-01 — SHIELD Canonical Terminology and Relational Architecture, version 0.1 for joint academic, sponsor, and researcher review. It converts the post-review architecture dictionary supplied on 14 August 2026 into a bounded, testable, and change-controlled proposal. It does not amend the governing scientific scope of Translation Engine Volume I and does not authorize a production system.
The requested decision is one of three dispositions:
Approve as a controlled architecture proposal for schema prototyping and Volume II development;
Approve with recorded conditions identifying changes, owners, evidence, and closure dates; or
Return for revision where terminology, authority, safety, feasibility, or research alignment remains insufficient.
Approval of ARC-01 means that the team may use its terms and interfaces in design notes and non-production prototypes. It does not mean that any architecture component is validated, secure, safe, interoperable, deployable, or commercially viable.
Executive finding
The supplied dictionary contains a coherent architectural direction: governed context packages, identity-aware resolution, declarative presentation, explicit human decisions, provenance, and an AI layer constrained to translation and drafting. Its strongest fit is as a future runtime architecture derived from the Volume I evidence program. Its principal defect is that several research hypotheses and design intentions were stated as accomplished engineering facts.
ARC-01 preserves the useful structure and corrects the overclaims. In particular, it:
makes Volume I the governing research foundation and assigns runtime engineering to Volume II;
replaces the assertion that every object has the same 16 fields with a shared governed envelope and typed packet payloads;
defines IADR as a policy decision model producing Permit, Deny, or Abstain;
recasts the “64-node mathematical Lock” as a 16-by-4 IADR conformance matrix, a coverage control rather than mathematical or cryptographic proof;
treats OCPs as versioned, evidence-backed representations rather than operational truth;
separates an IGP rule set from its runtime Semantic Experience Manifest;
limits HRDs to consequential human resolutions and describes them as tamper-evident until a complete signing and time-evidence design is selected and verified;
introduces explicit knowledge-promotion gates so observations, analytics, and AI drafts cannot silently become approved operational knowledge; and
converts cloud, latency, identity, cryptography, and BYO-LLM claims into measurable requirements or open decisions.
Authority relationship  [row end]

Instrument
Status in the program
Authority under ARC-01  [row end]

Translation Engine Volume I, final draft v1.0
Governing research foundation for 1 September–31 December 2026
Controls Phase 1 purpose, research boundary, evidence method, eight deliverables, OCP Profile 0.1, and Go / Revise / Stop decision.  [row end]

ARC-01 v0.1
Controlled architecture proposal
Defines corrected terminology, candidate runtime interfaces, conformance questions, and Volume II entry requirements. It cannot expand Phase 1 scope.  [row end]

Post-review canonical dictionary supplied 14 August 2026
Sponsor-supplied architecture input
Treated as a design proposition. Accepted, modified, deferred, or rejected propositions are recorded in Appendix B.  [row end]

Legacy architecture PDFs
Quarantined reference sources
May supply context or historical rationale only. They do not establish formal requirements, approvals, or evidence.  [row end]

Future Volume II
Not yet approved
Intended destination for approved production architecture, schemas, threat model, engineering decisions, benchmarks, verification evidence, and operating controls.

Project identity  [row end]

Field
Controlled value  [row end]

Project
Translation Engine applied-research program  [row end]

Project identifiers
Mitacs IT52870; University of Lethbridge FR173793  [row end]

Program period
1 September–31 December 2026  [row end]

Academic supervisor
Dr. Sidney Shapiro  [row end]

Industry sponsor and final deliverable acceptance authority
Stacey Malitowski  [row end]

Researcher
Noel Roemmele, University of Lethbridge employee  [row end]

Legal partner
Rugged Mobile Solutions Inc.  [row end]

Communication hub
Solid Stride Technology Partners Limited; not the contracting or governing partner  [row end]

Funding context
CAD 15,000 award: CAD 10,000 researcher allocation and CAD 5,000 research/materials budget; executed award records control

Immediate recommendation
ARC-01 should be reviewed and dispositioned before the project adopts a canonical technical vocabulary. If approved, the team should prototype only the common envelope, one OCP example, one IDP policy case, one IGP/manifest transformation, and one HRD event record against synthetic or approved data. Any broader runtime implementation remains contingent on Volume I findings and a separate Volume II authorization.

Figure 1. Proposed research-to-runtime architecture. Logical responsibilities are shown without asserting a production deployment topology.
2  Document Control and Use
Control record  [row end]

Field
Value  [row end]

Document identifier
ARC-01  [row end]

Title
SHIELD Canonical Terminology and Relational Architecture  [row end]

Version
0.1  [row end]

Status
Controlled Architecture Proposal — Joint Review Draft  [row end]

Issue date
14 August 2026  [row end]

Effective date
Not effective until approved  [row end]

Document owner
Project Steering Group  [row end]

Prepared for
Dr. Sidney Shapiro, Stacey Malitowski, and Noel Roemmele  [row end]

Legal entity
Rugged Mobile Solutions Inc.  [row end]

Classification
Project-controlled; no client data included  [row end]

Parent authority
Translation Engine Volume I v1.0  [row end]

Intended successor
Volume II approved architecture and engineering specification  [row end]

Change proposal
ARC-CP-001

Normative language
Within this proposal, shall identifies a requirement proposed for approval; should identifies a strong recommendation; and may identifies permission. These words do not become binding project requirements until ARC-01 is approved. Descriptive text uses “is” only for definitions or documented program facts, not for unverified performance or implementation claims.
Claim classes  [row end]

Class
Meaning
Required treatment  [row end]

Program fact
Established in supplied executed or approved project records
Cite the controlling record; do not enlarge its meaning.  [row end]

Volume I requirement
Governing Phase 1 research rule
Preserve unless changed through Volume I change control.  [row end]

Architecture decision
Proposed structural choice
Record rationale, alternatives, owner, approval, and verification.  [row end]

Engineering requirement
Proposed property of a future implementation
Assign measurable acceptance criteria and a test.  [row end]

Research hypothesis
Proposition requiring empirical study
Define evidence, counterevidence, uncertainty, and scope.  [row end]

Deferred concept
Potentially useful but premature
Keep outside canonical use until the named decision is resolved.  [row end]

Rejected claim
Misleading, infeasible, unsafe, or unsupported statement
Do not reproduce as a requirement or fact.

Supremacy and conflict rule
If ARC-01 conflicts with law, executed agreements, University of Lethbridge policy, ethics determinations, data-owner restrictions, or Volume I’s Phase 1 boundary, the higher authority controls and the conflict shall be logged. ARC-01 shall not be interpreted to authorize corpus access, personal-data processing, publication, software procurement, system integration, production use, or autonomous operational action.
Scope
ARC-01 covers terminology, conceptual layering, data-contract shape, lifecycle, decision semantics, presentation composition, human-resolution evidence, AI boundaries, security assumptions, non-functional requirements, verification strategy, and binder integration. It is deliberately technology-neutral where evidence or institutional decisions are incomplete.
Non-goals
ARC-01 does not:
select a production cloud or database;
assert a sub-100-millisecond service level;
define a complete cryptographic key-management system;
approve a model provider or unrestricted BYO-LLM use;
establish legal identity, employment, certification, or authorization records;
make an OCP an executable safety case or authorization token;
define a universal human-interface grammar;
permit automated promotion of observations or analytics into operational knowledge; or
replace the research design, schedule, deliverables, or acceptance gates in Volume I.
3  Research-to-Runtime Boundary
What Volume I establishes
Volume I authorizes a four-month design-science and corpus-research program. It defines eight controlled deliverables, including an OCP Research Requirements Profile 0.1. The profile is informative for research and has normative structural rules for Phase 1 examples; it is not a production schema, interoperability standard, executable authorization, regulatory control, or safety case.
The research architecture requires traceability from derived objects to sources, separation of source content from machine transformation and human adjudication, representation of authority and confidence as distinct properties, explicit conflict and missingness, bounded claims, abstention, versioning, ownership, and verification. Those invariants are inherited by ARC-01.
What ARC-01 adds
ARC-01 proposes the minimum conceptual contracts needed to test a future runtime without pretending it already exists. These contracts include a common governed envelope, packet-specific payloads, a tri-state IADR policy result, runtime composition boundaries, decision evidence, promotion gates, security assumptions, non-functional requirements, and test obligations.
Volume boundary rule  [row end]

Topic
Volume I
ARC-01
Future Volume II  [row end]

Corpus discovery and classification
Governing method and deliverables
No change
Consumes accepted artefacts only  [row end]

OCP Profile 0.1
Research representation with 16 sections
Preserved as the OCP payload profile
May evolve through evidence-backed schema governance  [row end]

IDP, IGP, HRD
Not established as Phase 1 deliverables
Defined as candidate typed packets
Formal schemas, services, controls, and tests  [row end]

IADR
Compatible contextual decision concept
Proposed decision model and conformance matrix
Executable policy model and verification evidence  [row end]

CRE, ECE, rendering kernel
Future requirements only
Defines logical responsibilities and interfaces
Components, deployments, APIs, failure modes, benchmarks  [row end]

Liquid Data
Not required
Candidate managed-data pattern
Selected products, topology, consistency, security, cost  [row end]

BYO-LLM
AI methods may be evaluated under controls
Allow-list policy pattern
Approved providers, routes, gateways, monitoring  [row end]

Cryptographic binding
Not claimed
Design prerequisites and terminology limit
Chosen algorithms, keys, trust anchors, timestamps, verification

Stage gates
The architecture shall move through distinct evidence gates:
Research gate: Volume I evidence supports the need and representational adequacy.
Concept gate: ARC-01 terms, boundaries, and open decisions are approved.
Schema gate: machine-readable schemas and validation suites pass synthetic tests.
Reference implementation gate: one bounded resolver/composer flow passes functional, security, privacy, accessibility, and failure tests.
Controlled evaluation gate: approved users and data demonstrate value over a baseline without unacceptable error or burden.
Production authorization gate: a separate accountable decision accepts residual risk, operating controls, support, cost, and legal obligations.
No gate may be inferred from completion of an earlier gate.
4  Architecture Principles and Invariants
Human authority
Consequential operational decisions remain with an authorized human unless a later, separately approved policy explicitly defines a narrow automated action. AI may retrieve, summarize, classify, draft, compare, or propose. It shall not invent authority, suppress uncertainty, silently change governing context, or convert a recommendation into a completed human decision.
“Human in the loop” is not sufficient by itself. The human shall receive enough information, time, authority, alternatives, explanation, and ability to decline or escalate for the review to be meaningful. Routine acknowledgements and passive display do not require HRDs; consequential choices do.
Evidence before claim
Every material assertion shall distinguish source evidence, deterministic transformation, statistical derivation, model output, human interpretation, and approved decision. A fluent AI output is not evidence. A checksum proves byte identity, not truth. A signature may provide origin and integrity evidence, not correctness or lawful authority.
Deterministic control boundary
Authorization, policy precedence, required confirmations, prohibited actions, and knowledge-promotion gates should be deterministic and testable. An LLM may help translate natural language into a candidate request, but the policy decision shall operate on validated structured inputs. If the structured intent cannot be established, the result is Abstain.
Explicit uncertainty and conflict
Unknown, stale, ambiguous, contradictory, unauthorized, or insufficiently evidenced inputs shall remain visible. The architecture shall not collapse competing authoritative assertions into a single answer without an authorized adjudication record. Confidence shall not substitute for authority.
Temporal validity
The architecture shall distinguish at least event time, observation time, record-creation time, effective time, and expiry or supersession time. A record may be authentic yet no longer applicable. Resolution shall use the policy and context versions effective for the decision, and the event log shall retain those versions.
Least privilege and purpose limitation
Access shall be constrained by subject, role, attributes, resource, action, environment, purpose, jurisdiction, sensitivity, and time. Possession of a valid identifier shall not grant access. Location shall never be the sole basis for trust.
Reversibility and correction
Approved releases may be immutable as historical records, but the system shall support correction by supersession, withdrawal, revocation, and archive. “Permanent” shall mean retained and auditable under an approved schedule, not impossible to correct or delete where law or agreement requires deletion.
Architecture invariants
Every packet has a globally or tenant-uniquely scoped identifier, type, schema version, lifecycle status, owner, sensitivity, provenance, and validation result.
Every consequential decision links the exact context, identity, policy, interface, and manifest versions presented.
Every policy decision returns Permit, Deny, or Abstain with machine-readable reason codes and an explanation suitable for the affected user.
Deny and Abstain are different: Deny means a determinative rule prohibits the action; Abstain means the system cannot make a reliable authorized decision.
No LLM output changes an approved packet, policy, identity attribute, or event record without an authorized review and release action.
Rendering cannot create new authority or hide a material conflict supplied by the resolver.
A presentation primitive shall not imply that the user must decide when no consequential choice exists.
Security claims shall identify the control, threat, trust boundary, implementation, and test evidence.
All performance targets shall state workload, percentile, measurement boundary, environment, and failure treatment.
Every automated transformation shall be reproducible or explicitly disclose why exact reproduction is impossible.
5  Corrected Canonical Data Dictionary
Canonical term policy
Terms in this chapter are proposed canonical definitions for architecture work after approval. Product names, historical names, metaphors, and aspirational phrases shall not override the defined meaning. Deprecated terms may appear in historical records only when tagged as deprecated and mapped to a current concept.  [row end]

Term
Proposed canonical definition
Must not mean or imply
Status  [row end]

Translation Engine
A governed ingestion and transformation pipeline that inventories approved sources, preserves provenance, produces structured graph assertions, and drafts candidate OCP artefacts for human validation and release.
A self-validating truth machine, production runtime, or autonomous authorizer.
Adopt with correction  [row end]

SHIELD
A working name for the future context-resolution, experience-composition, rendering, and decision-evidence architecture.
A deployed platform, operating system, safety certification, or registered standard.
Provisional name  [row end]

IADR
A four-dimension decision model: Intent, Authority, Dependencies, and Resolution. It frames whether a requested action is purposeful, authorized, contextually supportable, and capable of accountable closure.
A mathematical formula, cryptographic algorithm, or proof of safety.
Adopt as proposed model  [row end]

IADR Conformance Matrix
A 16-section by 4-dimension coverage matrix used to inspect whether an OCP example addresses each IADR dimension where applicable.
A “64-node lock,” security primitive, score of truth, or guarantee of correctness.
Adopt; replaces Lock claim  [row end]

Shield CPU
Historical metaphor for the policy and orchestration layer that applies IADR.
A literal processor, standardized algorithm, or independently verified mathematical mechanism.
Deprecated for formal specifications; “IADR Policy Decision and Orchestration Service” preferred  [row end]

Human First Principles
Requirements that consequential choices remain meaningfully human-governed, with understandable context, authority, alternatives, refusal, correction, escalation, and audit.
A claim that any nominal human click makes an unsafe system acceptable.
Adopt with operational criteria  [row end]

Operational Context Package (OCP)
A versioned, evidence-backed representation that binds operational purpose, actors, workflow, entities, context assertions, controls, dependencies, evidence, and rendering requirements within a declared scope.
Operational truth, executable permission, legal authority, safety case, or universal representation.
Adopt; Volume I controls Profile 0.1  [row end]

OCP Profile 0.1
The 16-section research requirements profile defined by Volume I for Phase 1 examples.
A common payload for every packet or a production interoperability standard.
Existing Volume I term  [row end]

Identity Packet (IDP)
A scoped, time-bounded set of verified or asserted subject, role, credential, delegation, session, and environmental attributes used as input to policy evaluation.
A master identity file, unrestricted personnel profile, or proof that every attribute is current.
Adopt as candidate packet  [row end]

Interaction Grammar Packet (IGP)
A versioned rule set governing information priority, permitted presentation primitives, action affordances, explanation, accessibility, localization, and failure states for a defined audience and use.
A rendered screen, user identity profile, or universal cognitive model.
Adopt as candidate packet  [row end]

Human Resolution Decision (HRD)
A tamper-evident event record of an authorized human’s consequential resolution, including what was presented, what was chosen, applicable versions, authority evidence, time evidence, and correction or escalation links.
Any click, an automatically generated approval, or a cryptographically bound record without a verified cryptographic design.
Adopt with narrowed boundary  [row end]

Operational Knowledge Graph (OKG)
A graph-oriented representation of entities, actors, activities, rules, states, sources, assertions, and provenance used for analysis and candidate package construction.
A single source of truth or a guarantee that extracted relations are correct.
Adopt  [row end]

Candidate Operational Observation
A source-linked, unapproved observation or proposed change awaiting verification, authority review, and disposition.
“Wisdom,” approved policy, or an automatic OCP update.
Adopt; replaces Wisdom OCM  [row end]

Analytical Context Artifact (ACA)
A derived, time-bounded analytical record containing metric definitions, population and denominator, method or model, uncertainty, validation, provenance, scope, and expiry.
A governing OCP, deterministic fact, or timeless risk score.
Adopt; replaces Analytical OCP  [row end]

Context Resolution Engine (CRE)
The logical service that validates a request, retrieves approved context and identity attributes, applies deterministic policy, resolves conflicts where authorized, and returns Permit, Deny, or Abstain with reasons and an evidence bundle.
A conversational LLM, simple IDP/OCP equality check, or universal truth resolver.
Adopt with correction  [row end]

Experience Composition Engine (ECE)
The logical service that transforms a permitted, evidence-qualified resolution bundle into a device-independent Semantic Experience Manifest using an approved IGP.
A policy decision point or physical renderer.
Adopt  [row end]

Semantic Experience Manifest
A runtime, device-independent instance specifying content, priority, state, permitted actions, explanations, accessibility semantics, and evidence references for one interaction.
The IGP itself, executable authority, or a device-specific screen.
Adopt  [row end]

Universal Rendering Kernel
A proposed client-side or edge rendering capability that interprets a supported manifest and composes approved primitives on a target device.
Proven universality, a browser engine replacement, or authorization logic.
Retain as provisional name  [row end]

Core
The highest-priority focal element for the present operational moment. It may display information or request an action.
A mandatory HRD trigger in every view.
Adopt with correction  [row end]

Ring
An ambient, non-interruptive representation of state, progress, boundary, or awareness.
A decorative status indicator without accessible alternative.
Adopt as provisional primitive  [row end]

Pads
Grouped contextual regions containing supporting evidence, controls, or related information.
Unbounded dashboard panels that compete with the Core.
Adopt as provisional primitive  [row end]

Dial
A governed lens for changing depth, time, scope, or perspective without altering underlying authority.
A free-form filter that hides mandatory evidence or changes a decision rule.
Adopt as provisional primitive  [row end]

Adaptive Operational Briefing (AOB)
A composite presentation envelope that binds Core, Ring, Pads, Dial, explanations, and action states for one operational moment.
A fifth primitive or an authorization artefact.
Adopt with correction  [row end]

Liquid Data Infrastructure
A technology-neutral managed-data pattern supporting governed, low-latency access to approved structured artefacts and event evidence.
A specific Azure product, a measured latency guarantee, or unrestricted data lake.
Retain as candidate pattern  [row end]

BYO-LLM
An allow-listed ability to use more than one approved model configuration behind a governed gateway and task-specific controls.
Any model, personal account, arbitrary prompt, unrestricted data transfer, or provider interchangeability without retest.
Adopt only with allow-list  [row end]

Abstain
A safe policy outcome used when intent, identity, authority, context, freshness, evidence, policy, or system condition is insufficient or conflicting.
Denial, error concealment, or a low-confidence guess.
Adopt

Deprecated terminology
The following terms shall not appear in new formal requirements except in a historical mapping: Stride AI, Shield OS, BJD-OS, “operational truth,” “mathematical Lock,” “64-node verification” as proof, “hidden Luma ID” as a security control, “permanent OCP” without lifecycle qualification, “Wisdom OCM,” and “analytical OCP.”
Terminology acceptance test
A term is ready for canonical approval when it has one definition, declared scope, clear non-meaning, owner, interfaces, measurable or reviewable conformance criteria, and no conflict with Volume I. Terms whose names imply unproven universality, security, mathematics, or deployment remain provisional even when their logical function is accepted.
6  Layered Architecture and Volume Crosswalk
Logical architecture
The architecture is a set of responsibilities and trust boundaries, not a mandatory microservice decomposition. A reference implementation may combine components if interfaces, evidence, policy separation, audit, and tests remain clear.
Source and evidence layer: approved raw documents, systems, images, records, and observations; immutable source captures where permitted; source authority and licence register.
Translation layer: inventory, parsing, OCR, normalization, semantic extraction, quality checks, human annotation, adjudication, and candidate graph assertions.
Knowledge layer: OKG assertions, provenance, conflict sets, controlled vocabularies, candidate observations, analytical artifacts, and released OCPs.
Resolution layer: request normalization, identity and context retrieval, policy evaluation, conflict handling, and Permit / Deny / Abstain result.
Composition layer: application of IGP rules to an approved result bundle, producing a Semantic Experience Manifest.
Presentation layer: rendering of an AOB through supported primitives and accessible alternatives.
Resolution-evidence layer: human response, HRD when consequential, event evidence, correction and escalation.
Learning-feedback layer: qualified events enter the Translation Engine as candidate evidence; they never bypass validation and release governance.
Component responsibility matrix  [row end]

Component
Inputs
Principal responsibility
Outputs
Explicit exclusion  [row end]

Translation Engine
Approved sources, source register, schemas, codebook, model configuration
Preserve sources and provenance; transform and propose structured assertions
OKG assertions, quality results, candidate OCPs, candidate observations
Final operational approval  [row end]

OKG
Released and candidate assertions with provenance
Represent relationships, conflicts, time, status, and lineage
Queryable evidence graph and subgraphs
Automatic authority hierarchy  [row end]

OCP service or repository
Approved OCP releases and lifecycle records
Validate, version, retrieve, supersede, withdraw, and archive OCPs
Exact versioned OCPs and validation evidence
Identity proof or policy decision  [row end]

IDP service or repository
Institutional identity and attribute sources
Produce scoped, minimum-necessary policy attributes
Time-bounded IDP and assurance information
Storing unrelated personnel intelligence  [row end]

IADR policy service
Normalized request, IDP, OCP, policy, environment
Evaluate Intent, Authority, Dependencies, and Resolution
Permit / Deny / Abstain, reason codes, evidence bundle
Natural-language invention of policy  [row end]

ECE
Permit result, evidence bundle, IGP, channel profile
Compose prioritized, accessible interaction semantics
Semantic Experience Manifest
Re-evaluating authority  [row end]

Rendering kernel
Valid manifest, device capabilities
Render supported primitives and capture interaction signals
Accessible AOB and user response
Creating undisclosed actions or context  [row end]

HRD recorder
Consequential response and exact interaction evidence
Validate and record human resolution
Tamper-evident HRD, event link, follow-up
Treating passive events as approvals  [row end]

Audit and observability service
Events from all components
Preserve trace, health, policy, security, and quality evidence
Logs, alerts, metrics, incident evidence
Becoming a shadow source of operational truth

Volume I deliverable crosswalk  [row end]

Volume I deliverable
ARC-01 dependency
Architecture use after acceptance
Prohibited shortcut  [row end]

D1 Corpus Boundary and Source Register
Defines which sources and authorities may feed Translation Engine work
Source authorization, scope, owner, cut-off, exclusion
Treating discoverable content as approved content  [row end]

D2 Reproducible Corpus Manifest
Supplies stable identifiers, checksums, provenance, sensitivity, and permitted use
Evidence links and acquisition trace
Loading unmanifested sources into model context  [row end]

D3 Metadata Schema, Taxonomy, and Codebook
Supplies controlled meanings and reliability evidence
OKG types, predicates, validation, annotation semantics
Treating an LLM label as a released taxonomy value  [row end]

D4 Workflow Comparison Set
Supplies bounded workflow structures and exceptions
OCP workflow and dependency payloads
Assuming a single workflow template is universal  [row end]

D5 Pattern Library
Supplies evidence-qualified reusable patterns
Candidate pattern references in OCPs and IGPs
Turning a recurring pattern into a mandatory rule without authority  [row end]

D6 AI-Assistance Evaluation
Supplies baseline comparison, error, review burden, privacy, cost, and reproducibility evidence
Determines whether and where LLM assistance is permitted
Adopting BYO-LLM because models are available  [row end]

D7 OCP Research Requirements Profile 0.1
Supplies the 16-section OCP payload profile
OCP examples and conformance matrix
Applying the same 16 sections to every packet  [row end]

D8 Final Research Report and Replication Package
Supplies results, limitations, artefact index, and Go / Revise / Stop recommendation
Determines whether Volume II should proceed
Treating ARC-01 approval as a Go decision

Dependency rule
An architecture concept may be designed before its supporting Volume I result exists, but it shall remain marked proposed and shall not be represented as evidence-backed. If Volume I produces negative or boundary-limited findings, Volume II shall narrow, revise, or retire affected concepts.
7  Common Governed Envelope and Lifecycle
Design rationale
Shared governance does not require identical domain payloads. OCPs, identity attributes, interaction rules, and decision evidence have different semantics, privacy risks, lifecycles, and validation needs. ARC-01 therefore defines a Common Governed Envelope (CGE) around typed payloads.
The envelope standardizes identity, versioning, status, ownership, time, sensitivity, provenance, validation, supersession, retention, and audit references. The payload schema defines packet-specific content. A packet is conformant only when both envelope and payload validate and the applicable policy review passes.
Envelope model  [row end]

Field group
Minimum content
Rule  [row end]

Identity
object type, object identifier, tenant or scope, schema identifier, schema version
Identifiers shall be stable within declared scope and shall not expose unnecessary personal information.  [row end]

Version and status
object version, lifecycle state, release identifier, compatibility class
Released objects shall not be silently overwritten.  [row end]

Accountability
owner, steward, creator, reviewer, approver, approval record
Roles shall be resolvable to controlled identities or functions.  [row end]

Time
created, observed, valid from, valid to, effective, expiry, superseded
Missing time semantics shall be explicit; all machine times use UTC with original zone retained where material.  [row end]

Classification
sensitivity, purpose, jurisdiction, disclosure rule, permitted uses
Minimum necessary data and purpose limitation apply.  [row end]

Provenance
source references, derivation activity, agent, transformation, evidence quality
Provenance shall distinguish source, machine, human, and approved decision.  [row end]

Integrity
canonicalization profile, digest algorithm and value, signature or timestamp references where used
Integrity metadata shall name algorithms and verification status; it shall not claim truth.  [row end]

Validation
structural result, semantic result, policy result, test suite version, unresolved defects
Failures shall block release according to severity policy.  [row end]

Relationships
supersedes, superseded by, derived from, depends on, related event, conflict set
Relationship direction and type shall be controlled.  [row end]

Retention and disposition
schedule, legal hold, archive, deletion or destruction eligibility
Retention shall follow controlling agreements and law, not an architectural preference for permanence.

Lifecycle

Figure 3. Governed lifecycle. Approved releases remain auditable; corrections occur by supersession or withdrawal.
The default governed lifecycle is:
Candidate: created or ingested; not approved for operational reliance.
Under review: assigned to reviewers; validation and evidence checks active.
Validated: required checks pass within a declared test boundary; approval is still pending.
Approved: accountable authority accepts the content and conditions.
Effective: the approved object is usable for its intended purpose and time window.
Superseded: a newer approved object replaces it prospectively; historical decisions retain their original reference.
Withdrawn or revoked: use is prohibited because authority, validity, safety, security, or correctness is compromised.
Archived or disposed: retained under archive controls or destroyed when permitted and required.
Transition controls  [row end]

Transition
Minimum gate evidence
Authorized actor
Failure outcome  [row end]

Candidate → Under review
Source and purpose identified; schema selected; sensitivity screened
Steward
Reject or quarantine  [row end]

Under review → Validated
Structural and semantic checks; provenance trace; conflict and time review
Qualified reviewer
Return to candidate  [row end]

Validated → Approved
Acceptance checklist; authority confirmation; open conditions recorded
Named approver
Conditional return or rejection  [row end]

Approved → Effective
Effective date, publication or deployment action, access rules
Release authority
Remain approved but inactive  [row end]

Effective → Superseded
Replacement approved; compatibility and migration impact assessed
Release authority
Continue current release  [row end]

Any active state → Withdrawn
Critical defect, revoked authority, incident, or data-owner direction
Designated incident or release authority
Block new use and notify affected owners  [row end]

Superseded/Withdrawn → Archived/Disposed
Retention and legal-hold check; evidence links preserved where required
Records/data authority
Retain under hold

Immutability and correction
The bytes of an approved release should be immutable. Corrections shall create a new version linked by supersedes or shall withdraw the defective version. Historical event evidence shall continue to reference the exact version used. Where privacy or contractual deletion is required, the disposition record shall preserve only the minimum lawful proof of deletion or unavailability.
Canonicalization and integrity
If JSON payloads are hashed or signed, a declared canonicalization method is required. RFC 8785 is an available JSON canonicalization scheme, but it is informational rather than an Internet Standards Track specification and therefore requires an explicit adoption decision and interoperability tests. A digest without canonicalization, algorithm identification, key or trust management where signing is used, and verification procedures is insufficient for a “cryptographically bound” claim.
8  Typed Packet Specifications
OCP packet
The OCP uses the CGE plus the exact 16-section payload already defined by Volume I Profile 0.1. ARC-01 does not rename or reorder those sections.  [row end]

No.
OCP payload section
Architecture interpretation  [row end]

1
Package metadata
Packet-specific metadata beyond the common envelope; no duplicate fields with conflicting values.  [row end]

2
Purpose and identity
Intended operational outcome, scope, non-goals, applicability, and limitations.  [row end]

3
Actors and roles
Operational roles, accountability, delegation, segregation, escalation, and affected parties; not live identity proof.  [row end]

4
Entities and assets
Governed objects, ownership, custody, lifecycle, and sensitivity.  [row end]

5
Workflows
Normal, exception, recovery, decision, and handoff paths with evidence.  [row end]

6
Inputs and outputs
Semantics, units, ownership, validation, and quality.  [row end]

7
Context variables and rules
Assertions, authority, observation and valid time, freshness, confidence, conflict, and relevance.  [row end]

8
State model
States, guarded transitions, invariants, invalid transitions, and terminal conditions.  [row end]

9
Risks, constraints, and controls
Harm, constraint, preventive and detective controls, residual risk, and evidence.  [row end]

10
Connectors and data boundaries
Systems of record, interfaces, identity, read/write boundary, and failure behavior.  [row end]

11
Brand and localization
Approved terms, language, locale, units, jurisdiction, brand, and accessible alternatives.  [row end]

12
Operational and visual assets
Content, forms, media, diagrams, licences, provenance, and accessibility metadata.  [row end]

13
Metrics and evidence
Outcome, process, guardrail, baseline, target, and evidence definition.  [row end]

14
Safety, privacy, and compliance
Applicable obligations, data categories, authority, prohibited uses, and review.  [row end]

15
Dependencies and assumptions
Services, people, policy, data, devices, assumptions, and validity conditions.  [row end]

16
Rendering specification
Priority, interaction intent, explanation, confirmation, accessibility, offline, empty, and error states.

An OCP release shall identify its evidence coverage and unresolved limitations. It shall not claim to be operational truth. A conformant OCP can still be incomplete, wrong, stale, unauthorized for a particular action, or unsuitable for a user.
IDP packet
The IDP shall contain only attributes required for declared policy decisions. Direct identifiers should remain in the authoritative identity provider where feasible; the packet should use a scoped pseudonymous subject identifier and assurance references.  [row end]

Payload group
Required or conditional fields
Key control  [row end]

Subject reference
scoped subject ID, tenant or organization, subject type
No email address as durable routing key; no global cross-context identifier unless justified.  [row end]

Identity assurance
issuer, authentication method, assurance level, authentication time, session
Authentication strength shall match action risk.  [row end]

Roles and attributes
roles, organization, job function, team, clearance or tier, employment or engagement status
Source and freshness required; tiers do not replace policy.  [row end]

Credentials
certification type, issuer, identifier, status, valid from/to, verification
Expired, suspended, or unverifiable credentials shall not authorize.  [row end]

Delegation
delegator, delegate, scope, start/end, constraints, revocation
Delegation cannot exceed delegator authority.  [row end]

Environment
device assurance, network posture, session risk, approved location attribute when necessary
Location is conditional context, not implicit trust.  [row end]

Consent and disclosure
notice, consent or alternative authority, disclosure constraints
Use only for the declared purpose.  [row end]

Revocation and validity
attribute expiry, revocation event, source availability
Stale critical attributes cause Deny or Abstain according to policy.

“Luma ID” may be retained as a product label only if it denotes a scoped, pseudonymous, rotatable identifier. The protected mapping to legal or institutional identity shall be access-controlled, auditable, purpose-limited, and separable from routine routing.
IGP packet
The IGP is a rule set, not a screen. It governs how an evidence bundle may be composed for an audience, action tier, channel, and accessibility context.  [row end]

Payload group
Minimum content
Test question  [row end]

Applicability
audience, workflow, action tier, channel, device capability, locale
Does the rule set apply to this moment?  [row end]

Information priority
mandatory facts, warnings, evidence, explanations, optional detail
Can required information be hidden or displaced?  [row end]

Primitive rules
permitted Core, Ring, Pads, Dial, AOB relationships
Are primitives used consistently and semantically?  [row end]

Action affordances
allowed actions, order neutrality, default behavior, confirmation
Is any action coerced, preselected, or misleading?  [row end]

Explanation
policy reason, provenance, uncertainty, conflict, recourse
Can the user understand why the system is asking or abstaining?  [row end]

Accessibility
semantic labels, focus order, keyboard, text alternatives, contrast, target size, timing, cognitive load
Does the experience meet the approved WCAG target and human-factors criteria?  [row end]

Localization and brand
approved terms, language, units, reading level, jurisdiction, brand
Are meaning and legal obligations preserved across locales?  [row end]

Exceptional states
Deny, Abstain, error, offline, stale, empty, interrupted, recovery
Does failure remain safe and understandable?  [row end]

Evidence capture
what is displayed, version, user response, timing, device, consent where required
Can a consequential decision be reconstructed?

Semantic Experience Manifest
The manifest is the runtime product of ECE composition. It shall include a manifest ID, event ID, IGP version, policy result reference, context bundle references, content blocks, semantic priority, accessibility semantics, permitted actions, confirmation requirements, expiry, offline rule, and integrity metadata. It shall not contain an action that was not permitted by the CRE result.
HRD packet
An HRD is created only when a human makes a consequential resolution: approval, rejection, exception, escalation, correction, consent, safety acknowledgement where policy requires it, or another decision that changes rights, obligations, safety posture, workflow state, or material resources.  [row end]

Payload group
Minimum content
Assurance purpose  [row end]

Event linkage
HRD ID, event ID, request ID, workflow instance
Links the decision to one operational moment.  [row end]

Actor and assurance
scoped subject ID, IDP version, authentication method and time, delegation
Shows which assured actor acted, without overexposing identity.  [row end]

Decision
decision type, selected option, options presented, decline or escalation availability
Preserves choice and counterfactual options.  [row end]

Evidence presented
OCP, policy, IGP, manifest and analytical artifact versions; material warnings and conflicts
Reconstructs the decision basis.  [row end]

Authority result
Permit result, reason codes, policy version, unresolved conditions
Shows the system’s authorization judgment.  [row end]

Time and environment
event, presentation and decision times; device/session; zone; offline status
Supports sequence and validity analysis.  [row end]

Human statement
acknowledgement, reason or comment where required, correction request
Preserves meaningful human input.  [row end]

Integrity evidence
canonicalization, digest, signature or timestamp reference, verification status
Supports tamper detection; does not prove correctness.  [row end]

Follow-up
resulting state, tasks, notifications, escalation, superseding HRD, revocation or correction
Prevents the record from being a dead-end approval token.

Until a complete cryptographic design passes independent verification, formal text shall say tamper-evident HRD rather than “cryptographically bound HRD.”
Candidate Operational Observation
A candidate observation shall contain source, observer or system agent, observed time, subject, proposed assertion or change, confidence and method, sensitivity, affected OCP or rule, urgency, and status. It may originate from field input, system events, incident review, audit, or analysis. It shall enter a review queue; it shall not update an approved OCP automatically.
Analytical Context Artifact
An ACA shall include the analytical question, population, cohort, denominator, unit, method or model, data and feature versions, exclusions, uncertainty, calibration where relevant, validation, fairness or subgroup analysis where people may be affected, intended and prohibited use, effective window, expiry, provenance, and reviewer. A risk score without these fields shall not be treated as decision-grade evidence.
9  IADR Decision Model
Purpose
IADR is a structured way to ensure that a request is not acted upon merely because content exists. It combines purpose, permission, situational sufficiency, and accountable closure. It is not an equation and it does not guarantee a correct outcome.  [row end]

Dimension
Question
Minimum evidence
Typical failure  [row end]

Intent
What outcome is requested, by whom, for what purpose, within what action and scope?
normalized action, target resource, declared purpose, workflow state, request source
ambiguous query, prohibited purpose, action outside workflow  [row end]

Authority
Is this actor or service permitted to perform this action under current policy?
assured subject, roles/attributes, credentials, delegation, policy, jurisdiction, separation of duties
expired credential, insufficient role, self-approval conflict  [row end]

Dependencies
Are required context, prerequisites, systems, data quality, safety controls, and temporal conditions satisfied?
exact OCP, current state, prerequisite events, freshness, system health, conflict set
stale state, missing prerequisite, contradictory authoritative sources  [row end]

Resolution
Can the action be closed responsibly, recorded, corrected, escalated, and monitored?
permitted options, confirmation, HRD rule, rollback or recovery, owner, event evidence
no authorized closer, irreversible action without confirmation, logging unavailable

Decision outcomes  [row end]

Outcome
Meaning
Required response  [row end]

Permit
All mandatory rules resolve affirmatively for the requested action and declared context.
Return permitted action set, constraints, reason codes, evidence bundle, expiry, and required confirmation.  [row end]

Deny
A determinative valid rule prohibits the action.
Block the action; identify the controlling rule and permissible recourse without disclosing protected information.  [row end]

Abstain
The system cannot make a reliable authorized decision because required input, authority, evidence, freshness, policy, or service is missing, ambiguous, conflicting, or untrusted.
Take no consequential action; explain the insufficiency; request clarification, refresh, or escalate to a named role.

Precedence
The default precedence is law and executed authority → institutional and data-owner rules → safety and privacy constraints → action-specific policy → workflow and context rules → presentation preference. A lower-precedence rule cannot override a higher-precedence prohibition. If precedence itself is unclear, the result is Abstain.
Evaluation logic
Validate request syntax, scope, source, purpose, and time.
Retrieve exact policy, OCP, IDP attributes, current state, dependencies, and relevant analytical artifacts.
Reject invalid or untrusted objects before policy evaluation.
Evaluate determinative prohibitions. A satisfied prohibition produces Deny.
Evaluate mandatory evidence and freshness. Missing or conflicting critical evidence produces Abstain unless policy explicitly defines a safe default.
Evaluate authority, delegation, separation of duties, and action tier.
Evaluate dependency and resolution requirements, including confirmation, logging, recovery, and escalation.
Produce Permit only if all mandatory conditions pass.
Return a machine-readable decision object containing reason codes, exact versions, validity window, obligations, and explanation data.
Reason-code families  [row end]

Family
Examples
Default result  [row end]

INT
INT-AMBIGUOUS, INT-PURPOSE-PROHIBITED, INT-OUT-OF-SCOPE
Abstain or Deny according to policy  [row end]

AUT
AUT-NOT-AUTHENTICATED, AUT-ROLE-MISSING, AUT-CREDENTIAL-EXPIRED, AUT-DELEGATION-INVALID, AUT-SEPARATION-CONFLICT
Deny when determinative; otherwise Abstain  [row end]

DEP
DEP-CONTEXT-MISSING, DEP-STALE, DEP-CONFLICT, DEP-PREREQUISITE, DEP-SYSTEM-UNAVAILABLE
Abstain  [row end]

RES
RES-NO-CLOSER, RES-LOGGING-UNAVAILABLE, RES-CONFIRMATION-MISSING, RES-RECOVERY-UNDEFINED
Abstain or Deny for prohibited irreversibility  [row end]

POL
POL-NOT-FOUND, POL-VERSION-MISMATCH, POL-PRECEDENCE-CONFLICT
Abstain  [row end]

SEC
SEC-INTEGRITY-FAIL, SEC-DEVICE-UNTRUSTED, SEC-SESSION-RISK, SEC-INCIDENT-HOLD
Deny or Abstain according to incident policy

IADR conformance matrix
The matrix evaluates whether each of the 16 OCP sections addresses each IADR dimension where applicable. The resulting 64 cells are marked Satisfied, Partial, Not Applicable with rationale, Failed, or Not Tested. No numeric total shall be described as safety, truth, or authorization. A critical failed cell can block a release even when all other cells pass.  [row end]

Cell content
Required entry  [row end]

Applicability
applicable / not applicable with justification  [row end]

Requirement
the specific IADR-related requirement  [row end]

Evidence
source, test, review, or policy reference  [row end]

Result
satisfied / partial / failed / not tested  [row end]

Severity
critical / major / minor / observation  [row end]

Owner and disposition
responsible role, due date, waiver or correction record


Figure 2. IADR tri-state decision model. The four dimensions are evaluated through deterministic policy and do not constitute a mathematical or cryptographic proof.
10  Corrected Runtime Relational Sequence
Normal sequence
Trigger. A human, workflow, system event, or approved service initiates a request. Voice or chat through an approved LLM is only one possible channel.
Request boundary. The gateway assigns an event and request identifier and records source, intent candidate, time, environment, channel, and component versions. Natural language is transformed into a candidate structured request and validated.
Resolution context. The CRE retrieves the minimum necessary IDP attributes, exact OCP release, current operational state, policy, dependency evidence, and relevant analytical artifacts from approved repositories.
IADR decision. Deterministic policy evaluates Intent, Authority, Dependencies, and Resolution and returns Permit, Deny, or Abstain with reasons, obligations, versions, and expiry.
Composition. For Permit, ECE applies the approved IGP to the evidence bundle and creates a Semantic Experience Manifest. Deny and Abstain receive their own governed manifests for explanation and recourse.
Render. The rendering kernel validates the manifest and produces an accessible AOB using supported Core, Ring, Pads, and Dial semantics. It cannot add actions or suppress mandatory evidence.
Human response. The user acknowledges, declines, chooses, corrects, requests clarification, or escalates. A consequential resolution creates an HRD; ordinary navigation or passive viewing does not.
Evidence closure. The event and, where applicable, HRD enter a tamper-evident audit record with exact input, policy, OCP, IGP, and manifest versions and the resulting workflow state.
Candidate feedback. Qualified event evidence may be transformed into a candidate operational observation or analytical artifact.
Knowledge promotion. No candidate becomes an approved OCP, rule, taxonomy value, credential, or pattern without provenance, validation, human authority, quality checks, versioning, and controlled release.
Exception paths  [row end]

Condition
Required behavior
Prohibited behavior  [row end]

Ambiguous natural-language request
Ask a bounded clarification or Abstain
Guess the action or target  [row end]

Identity provider unavailable
Use an expressly approved cached attribute set within its validity window or Abstain
Reuse stale identity indefinitely  [row end]

OCP conflict
Present the conflict or route to authorized adjudication
Select the most convenient source silently  [row end]

Policy unavailable or version mismatch
Abstain and alert operations
Default to Permit  [row end]

Renderer cannot support required accessibility or confirmation
Use approved alternative channel or Abstain
Render a materially incomplete experience  [row end]

Audit or HRD recorder unavailable for an action requiring evidence
Abstain or enter an approved fail-safe mode
Perform the action and reconstruct the record later  [row end]

Offline operation
Apply explicit offline policy, cached-version expiry, queued evidence, and reconciliation rules
Treat local cache as current without qualification  [row end]

User declines or escalates
Preserve the response and route appropriately
Convert decline into inactivity or approval  [row end]

Integrity verification fails
Quarantine the object, Deny or Abstain, and alert
Continue using the object because its content appears plausible

Feedback-loop protections
The system shall prevent circular self-validation. A model-generated observation cannot cite its own generated OCP as independent evidence. An event caused by a recommendation is not proof that the recommendation was correct. Analytics derived from prior HRDs shall not be used to pressure future users or infer worker quality without a separately approved purpose and methodology. Training or retrieval datasets shall preserve origin, consent or authority, time, and exclusions.
11  AI-Assisted Translation and Knowledge Promotion
Permitted role
Within Phase 1, approved AI methods may support bounded research tasks such as extraction, candidate classification, comparison, drafting, or retrieval evaluation. They shall be compared with credible non-AI baselines on held-out data and assessed for severe error, abstention, review effort, reproducibility, privacy, security, and cost as required by Volume I D6.
In a future runtime, an LLM may translate conversational input into a candidate structured request and explain deterministic results in controlled language. The LLM shall not be the policy decision point, identity authority, system of record, or unreviewed knowledge-release authority.
Allow-list model
“BYO-LLM” shall mean selection from approved configurations, not unrestricted provider choice.  [row end]

Control field
Required decision  [row end]

Provider and product
legal entity, service, support channel, contract  [row end]

Model configuration
model name, exact version or release channel, endpoint, parameters, tools, system prompt  [row end]

Account and tenancy
institutional or approved enterprise account; administrative owner; access roles  [row end]

Region and routing
processing and storage regions; cross-border transfer; subprocessors  [row end]

Data classes
permitted, prohibited, and transformation-required data; client-specific restrictions  [row end]

Retention and training
prompt/output retention; provider training or human review; opt-out evidence  [row end]

Security
encryption, authentication, logging, incident notification, vulnerability process  [row end]

Privacy and deletion
data-subject handling where applicable, deletion, export, closure  [row end]

Reproducibility
version capture, prompt and parameter record, seed where meaningful, test date  [row end]

Quality and guardrails
task-specific baseline, severe-error threshold, abstention, human review  [row end]

Cost and availability
budget cap, rate limits, continuity, fallback, termination export  [row end]

Approval and expiry
approving roles, effective window, review date, suspension trigger

Context minimization
The gateway shall send only the minimum approved context required for the task. Prompt construction shall preserve object identifiers and versions without disclosing unnecessary client, employee, customer, credential, location, or free-text data. Retrieval filters are a control but not sufficient by themselves; service terms, logging, export, and administrative access also require approval.
Knowledge-promotion gate  [row end]

Gate
Question
Evidence
Failure disposition  [row end]

Source authority
Is the source permitted and within the declared boundary?
D1 and D2 references; licence or access term
Quarantine or exclude  [row end]

Provenance
Can each assertion be traced through transformations and agents?
PROV-compatible lineage; logs; checksums
Return for repair  [row end]

Structural validity
Does the object satisfy its schema and constraints?
JSON Schema and graph validation
Reject candidate  [row end]

Semantic quality
Is meaning accurate, scoped, temporally valid, and conflict-aware?
Reviewer evidence; domain comparison; uncertainty
Revise or reject  [row end]

Independent review
Has required second review or adjudication occurred?
Reviewer identity, result, disagreement record
Hold candidate  [row end]

Authority
Does the approver have authority for this object and purpose?
role, delegation, approval record
Reject approval  [row end]

Safety/privacy/security
Are applicable controls and prohibited uses resolved?
assessments, tests, conditions
Hold or withdraw  [row end]

Release
Are version, effective time, access, retention, and rollback defined?
release checklist
Remain approved but inactive

Model and prompt change
A change in model, version, endpoint, prompt, tool configuration, retrieval corpus, safety setting, or output parser can change results. Material changes shall trigger regression tests against a frozen benchmark and a new configuration approval. Provider claims of equivalence are not sufficient.
AI risk frame
NIST’s AI Risk Management Framework is a voluntary framework organized around Govern, Map, Measure, and Manage. ARC-01 uses it as a reference for accountable scoping, measurement, risk treatment, monitoring, and documentation; it makes no certification claim. The NIST Generative AI Profile should inform risks specific to generative systems, including confabulation, data privacy, information integrity, misuse, and human over-reliance.
12  Security, Privacy, Legal, and Identity Assumptions
Security posture
ARC-01 assumes zero implicit trust from network location, device ownership, or possession of a packet. Authentication and authorization are distinct. Every request is evaluated for subject, device or session where appropriate, resource, action, environment, purpose, and current policy. This is consistent with the resource-focused principles in NIST SP 800-207 but does not constitute a Zero Trust Architecture implementation claim.
Trust zones  [row end]

Zone
Example content
Default control posture  [row end]

Source evidence zone
client documents, images, exports, system records
read-only acquisition where feasible; owner restrictions; strong access and audit  [row end]

Research workspace
normalized corpus, annotations, notebooks, held-out sets
project access; separation of sensitive and de-identified data; versioning; backup  [row end]

Controlled knowledge zone
released taxonomy, OKG assertions, OCPs, IGPs, policies
release authority; schema validation; integrity evidence; least privilege  [row end]

Identity and policy zone
IDP attributes, credentials, delegation, policy
minimum disclosure; high assurance; revocation; separation of duties  [row end]

Runtime presentation zone
manifests, cached context, device events
minimum necessary content; expiry; accessible secure rendering; device controls  [row end]

Audit and evidence zone
requests, policy results, HRDs, verification and incident records
append-oriented/tamper-evident controls; restricted access; retention; monitoring  [row end]

External AI service zone
approved prompts and outputs
allow-listed configuration; content filter; contractual controls; no unapproved data

Identity requirements
Use institutionally or contractually authoritative identity sources.
Use scoped pseudonymous identifiers for routine routing and logs where feasible.
Protect and audit the mapping to direct identity.
Make identifier rotation and account-merger rules explicit.
Verify roles, credentials, employment or engagement status, and delegations at an appropriate freshness.
Separate identity proofing, authentication, attribute issuance, policy decision, and audit responsibilities.
Treat Tier 1–4 labels as attributes within policy, not as universal authority.
Do not collect location unless it is necessary, lawful, proportionate, accurate enough, and bounded by retention and disclosure rules.
Attribute-based authorization
The proposed authorization model is attribute-based: subject, object, action, and environment attributes are evaluated against policy. This aligns conceptually with NIST SP 800-162. Implementation shall still define policy language, authoritative attribute sources, conflict and freshness rules, decision caching, obligations, explainability, and test coverage.
Privacy and anonymization
Existing client agreements and anonymization features are relevant controls but do not eliminate the need to verify data flow. “Anonymized” shall not be asserted solely because direct names are removed. The team shall document transformation, residual re-identification risk, linkage risk, free-text and image handling, access, retention, and whether data can be reconnected through protected mappings or external information.
No client data is included in ARC-01. Before runtime prototyping with real data, DAT-01 shall identify owner, purpose, permitted use, classification, data path, anonymization or pseudonymization method, residual risk, access, retention, incident path, and evidence of authority for each source class.
Legal and institutional boundary
Executed University, sponsor, client, confidentiality, intellectual-property, publication, authorship, and engagement records control. ARC-01 does not interpret or replace those instruments. The program register should identify the controlling document for background IP, newly created IP, code, schemas, annotations, patterns, confidential information, publication review, authorship, commercial use, and data disposition.
Tamper evidence and cryptography
A defensible cryptographic claim requires:
a canonical byte representation;
named digest and signature algorithms and parameter profiles;
key generation, storage, access, rotation, recovery, revocation, and destruction;
signer and verifier trust anchors;
trusted time or an explicitly bounded clock model;
verification at creation and later audit;
algorithm-agility and migration;
failure, compromise, and incident procedures; and
independent implementation and interoperability tests.
RFC 3161 describes a Time-Stamp Protocol through which a Time Stamping Authority can provide evidence that a datum existed before a particular time. It is a possible component, not an automatic program requirement. The selected architecture may use another controlled time-evidence approach if it meets the stated assurance need.
Threats requiring explicit treatment  [row end]

Threat
Example
Required design response  [row end]

Prompt injection or source manipulation
malicious text instructs a model to ignore controls
isolate source content from instructions; validate outputs; deterministic policy boundary  [row end]

Poisoned or misleading corpus content
obsolete procedure appears authoritative
source authority, time, conflict, reviewer, withdrawal  [row end]

Privilege escalation
role attribute or delegation is forged or stale
authoritative attributes, short validity, revocation, policy test  [row end]

Replay
old Permit or HRD reused for a new state
event nonce or unique ID, expiry, current-state binding, replay detection  [row end]

Manifest tampering
renderer receives altered action set
integrity verification and deny/abstain on failure  [row end]

Sensitive-data leakage
restricted client content enters external LLM logs
data-class gateway, redaction, contractual controls, monitoring  [row end]

Model substitution
provider silently changes model behavior
configuration inventory, regression tests, suspension thresholds  [row end]

Audit suppression
consequential action occurs while logging is unavailable
fail-safe policy, monitoring, reconciliation, incident procedure  [row end]

Misleading interface
warning hidden or default biases the user
IGP constraints, accessibility and human-factors tests, exact manifest evidence  [row end]

Re-identification
combined pseudonymous records reveal a person
minimization, separation, aggregation, access limits, residual-risk review

13  Non-Functional Requirements and Verification
Status of requirements
The following are proposed baseline requirements. Numeric targets are placeholders for approval only where marked “TBD by benchmark”; ARC-01 deliberately does not inherit the unsupported sub-100-millisecond claim.  [row end]

ID
Requirement
Proposed measure or acceptance rule
Verification
Owner
Status  [row end]

NFR-01
Decision correctness
100% pass on determinative policy conformance suite; no unauthorized Permit in critical negative tests
automated policy tests and independent review
Technical lead / Academic PI
Proposed  [row end]

NFR-02
Safe abstention
All defined missing, stale, conflict, or untrusted critical-input cases return Abstain or Deny as policy specifies
negative and fault-injection tests
Technical lead
Proposed  [row end]

NFR-03
Trace completeness
Each decision links request, policy, IDP, OCP, IGP/manifest, result, reason, and event versions
trace query and sample reconstruction
Quality lead
Proposed  [row end]

NFR-04
Provenance
Every promoted assertion traces to permitted source and derivation activity
lineage validation and sample audit
Data steward
Proposed  [row end]

NFR-05
Temporal correctness
Resolver uses applicable effective versions and detects expired critical inputs
boundary-time and clock tests
Technical lead
Proposed  [row end]

NFR-06
Availability
Service-specific objective to be set after action-tier and offline analysis; no blanket target
load, failover, and recovery tests
Operations owner
Open target  [row end]

NFR-07
Latency
Percentile targets measured end-to-end by scenario, payload, network, cache, and action tier; TBD by benchmark
controlled benchmark with p50/p95/p99 and errors
Engineering lead
Open target  [row end]

NFR-08
Scalability
Defined throughput and corpus size supported without violating correctness or cost guardrails
load and capacity test
Engineering lead
Open target  [row end]

NFR-09
Consistency
Policy, identity, and OCP consistency model declared; stale reads bounded and observable
concurrency and version tests
Architecture owner
Proposed  [row end]

NFR-10
Security
Threat model complete; critical findings closed; least privilege and integrity failures tested
threat review, security tests, penetration test before production
Security authority
Proposed  [row end]

NFR-11
Privacy
Data inventory, purpose, minimization, disclosure, retention, and residual re-identification risk reviewed
privacy assessment and data-flow test
Data/privacy owner
Proposed  [row end]

NFR-12
Accessibility
User-facing experiences target WCAG 2.2 AA plus documented cognitive and field-use requirements
automated and expert manual accessibility evaluation
Accessibility owner
Proposed  [row end]

NFR-13
Usability
Consequential users understand action, reason, alternatives, and recourse at approved thresholds
scenario-based human evaluation
Research lead
Open target  [row end]

NFR-14
Reproducibility
Reference test outputs can be reproduced from frozen artefacts within stated tolerance
independent reproduction
Academic PI / reviewer
Proposed  [row end]

NFR-15
Interoperability
Declared schema profiles validate across at least two independent implementations before interoperability claim
conformance and round-trip tests
Architecture owner
Proposed  [row end]

NFR-16
Portability
Core packets and event exports use documented non-proprietary representations; provider-specific fields isolated
migration and export test
Architecture owner
Proposed  [row end]

NFR-17
Recoverability
Recovery-point and recovery-time objectives set by data class and action tier; restoration verified
backup restore and disaster-recovery exercise
Operations owner
Open target  [row end]

NFR-18
Observability
Health, decision outcomes, abstentions, failures, policy versions, and cost are measurable without exposing excess personal data
telemetry review and alert test
Operations / privacy
Proposed  [row end]

NFR-19
Maintainability
Schema, policy, component, and dependency changes use version control, review, tests, and rollback
change audit
Engineering lead
Proposed  [row end]

NFR-20
Cost control
Unit-cost metrics and monthly budget ceilings defined; abnormal use alerted
cost benchmark and forecast
Sponsor / operations
Open target  [row end]

NFR-21
Offline safety
Each action tier declares whether offline use is prohibited, read-only, or queued with reconciliation
offline and reconnect scenarios
Architecture owner
Proposed  [row end]

NFR-22
Localization
Terminology, units, dates, reading level, and legal text remain semantically correct across approved locales
linguistic and domain review
Product / domain owner
Proposed  [row end]

NFR-23
Audit retention
Retention, legal hold, access, and disposition rules are defined by record class
records audit and disposition test
Records/data owner
Proposed  [row end]

NFR-24
Cryptographic agility
Integrity profiles identify algorithms and migration; compromised algorithms can be retired
configuration review and rotation exercise
Security authority
Proposed

Performance requirement form
Every latency or throughput requirement shall state scenario, user population, request mix, payload size, cache state, network, client device, consistency level, percentile, warm-up, observation window, error rate, timeout behavior, and measurement boundary. “Sub-100 ms” is not a valid requirement without these qualifiers and should not be made a program promise before benchmarking.
Accessibility basis
WCAG 2.2 defines testable, technology-independent success criteria under the principles Perceivable, Operable, Understandable, and Robust. The future interface should target Level AA unless a controlling institutional requirement is stronger. Conformance alone is not sufficient for field safety or cognitive usability; representative scenario tests shall also address gloves, glare, noise, fatigue, connectivity, interruption, literacy, time pressure, and accessible alternatives.
14  Conformance and Test Strategy
Test layers  [row end]

Layer
Purpose
Minimum evidence before approval  [row end]

Schema
Confirm envelope and typed payload structure
positive, negative, boundary, required-field, type, enum, pattern, and version tests  [row end]

Semantic
Confirm meaning, units, authority, time, and relationship integrity
codebook examples, expert review, constraint tests, conflict cases  [row end]

Provenance
Confirm lineage and transformation trace
source-to-assertion and assertion-to-release traversal  [row end]

Policy
Confirm IADR results and precedence
decision tables, determinative negative cases, separation-of-duty and delegation tests  [row end]

Lifecycle
Confirm allowed transitions, supersession, withdrawal, and archive
state-transition and historical reconstruction tests  [row end]

Security
Confirm threat controls and fail-safe behavior
authentication, authorization, integrity, injection, replay, logging, incident tests  [row end]

Privacy
Confirm minimization, data flow, disclosure, retention, and deletion
data-flow inspection, access tests, re-identification analysis  [row end]

Composition
Confirm ECE applies IGP without altering authority
golden manifests, prohibited-action and mandatory-content tests  [row end]

Rendering
Confirm semantic fidelity and accessibility across supported devices
visual, semantic, keyboard, assistive-technology, offline/error tests  [row end]

HRD
Confirm consequential decision evidence and correction
reconstruction, replay, integrity, time, correction, and revocation tests  [row end]

Resilience
Confirm safe behavior under dependency failure and stale data
fault injection, failover, timeout, queue, reconnect tests  [row end]

Human factors
Confirm users understand, decide, decline, and recover
representative moderated scenarios and severe-use-error analysis  [row end]

Reproducibility
Confirm independent rerun from frozen artefacts
environment record, exact versions, scripts, expected results, discrepancy log

Gate outcomes
Tests shall return Pass, Conditional Pass, Fail, or Not Tested. Conditional Pass requires named conditions, risk owner, due date, restricted use, and retest. A critical Fail or critical Not Tested blocks release. Test counts and pass percentages shall not conceal untested critical behaviors.
Minimum reference scenario set
authorized normal action with current evidence;
determinative Deny for insufficient authority;
Abstain for missing critical context;
Abstain for conflicting authoritative sources;
expired credential and revoked delegation;
stale OCP and policy version mismatch;
system-of-record unavailable;
integrity failure and replay attempt;
user decline, correction, and escalation;
consequential action requiring HRD;
informational display requiring no HRD;
accessible keyboard and assistive-technology path;
offline read-only and reconnect reconciliation;
LLM ambiguity, prompt injection, and fabricated citation;
superseded and withdrawn OCP behavior; and
historical reconstruction of a completed event.
Traceability rule
Every approved architecture requirement shall link to one or more tests and every test shall link to a requirement, threat, user need, or research question. Orphan requirements and orphan tests are defects. The trace matrix shall include requirement version, test version, environment, result, evidence location, reviewer, date, open issue, and disposition.
15  Open Questions and Decisions Required
Decision register  [row end]

ID
Decision
Why it matters
Options to evaluate
Accountable role
Required by  [row end]

ARC-D01
Approve “SHIELD” as program architecture name
Avoids branding and scope confusion
approve; rename; retain as working label
Stacey Malitowski with Dr. Shapiro consultation
Concept gate  [row end]

ARC-D02
Retire “Shield CPU” from formal specifications
Metaphor currently implies hardware and mathematical assurance
retire; retain historical alias; formally redefine
Architecture owner / Dr. Shapiro
ARC-01 approval  [row end]

ARC-D03
Approve IADR semantics and precedence
Controls every future authorization decision
approve; revise dimensions; choose another policy model
Dr. Shapiro and technical reviewer
Schema gate  [row end]

ARC-D04
Confirm OCP Profile 0.1 evidence after Volume I D7
Prevents architecture from outrunning research
adopt; revise; stop
Dr. Shapiro / Stacey Malitowski
Final Phase 1 gate  [row end]

ARC-D05
Select authoritative identity and attribute sources
IDP reliability depends on source and freshness
University, partner, federated, or use-case-specific
Institutional/security authority
Reference implementation  [row end]

ARC-D06
Decide Luma ID naming and scope
Prevents pseudonym from becoming a global tracker
product label; neutral subject ID; no persistent ID
Privacy/security authority
IDP schema  [row end]

ARC-D07
Define HRD materiality boundary
Avoids over-recording and approval theatre
action-tier matrix and exceptions
Dr. Shapiro / Stacey Malitowski
HRD schema  [row end]

ARC-D08
Select cryptographic and trusted-time profile
Required before “cryptographically bound” claim
JCS + signature + RFC 3161; platform service; other
Security authority
Engineering design  [row end]

ARC-D09
Select structured data infrastructure
Determines consistency, cost, region, and operations
relational, graph, document, hybrid managed services
Technical lead / sponsor
Volume II plan  [row end]

ARC-D10
Set scenario-specific performance targets
Prevents arbitrary latency promise
benchmark-derived targets by action tier
Technical lead / user research
Post-prototype benchmark  [row end]

ARC-D11
Approve AI services and gateway
Controls data exposure and reproducibility
institutional list and task-specific configurations
Dr. Shapiro / institutional authority
Before AI use  [row end]

ARC-D12
Define second-review capacity
D3 reliability and independent review need a committed method
Dr. Shapiro, trained second coder, independent reviewer
Dr. Shapiro
Before reliability pilot  [row end]

ARC-D13
Define data retention and event evidence schedule
Affects privacy, audit, cost, and correction
record-class schedules
Data owner / institution
Before real data  [row end]

ARC-D14
Assign Volume II architecture owner
Prevents diffuse decision rights
named technical lead, architecture board, external review
Stacey Malitowski / Dr. Shapiro
Before Volume II  [row end]

ARC-D15
Determine legal name and status of each collaborating entity in artefacts
Prevents Stride/Rugged misrepresentation
Rugged as legal partner; Solid Stride communication role only
Stacey Malitowski
Immediate

Unknowns that shall remain explicit
The approved collaboration/version-control/annotation/AI tool list has not yet been received. The exact second-coder method and committed capacity are not yet known. Planned industrial partners, future licences, technology-transfer routes, and future funding applications remain planning hypotheses. Those matters shall not be converted to document facts until an authoritative record is filed.
16  Change Impact and Implementation Roadmap
Controlled implementation sequence  [row end]

Phase
Timing
Purpose
Minimum output
Exit criterion  [row end]

A — Concept disposition
Before 1 September where practicable
Review ARC-01 terms, authority, and boundaries
approval record, conditions, open-decision owners
joint disposition recorded  [row end]

B — Research alignment
September–December 2026
Use ARC-01 only as a lens on Volume I evidence
crosswalk updates, schema questions, synthetic examples
no expansion of eight deliverables  [row end]

C — Schema prototype
After relevant Volume I evidence or explicitly as bounded research
Test CGE, typed packets, lifecycle, and validation
JSON Schemas, examples, test suite, decision log
structural and negative tests pass  [row end]

D — Reference resolver/composer
Only after schema and policy approval
Implement one synthetic or approved low-risk flow
CRE/ECE reference path, manifest, HRD, audit
security, accessibility, policy, and reconstruction tests pass  [row end]

E — Controlled evaluation
After institutional and data authorization
Compare user and operational outcomes with baseline
protocol, evaluation, limitations, risk update
evidence supports Go / Revise / Stop  [row end]

F — Volume II adoption
Separate approval
Produce production architecture and operating plan
approved Volume II, threat model, NFRs, support and cost
accountable production authorization

Binder change and integration register  [row end]

Binder component
Required change
ARC-01 relationship
Priority
Owner / reviewer  [row end]

BND — Master Binder Register
Add ARC-01 under controlled architecture proposals; record ARC-CP-001; list status and approvals
ARC-01 is subordinate to Volume I
Immediate
Noel / Stacey  [row end]

Administrative Fact Sheet
Use Rugged Mobile Solutions Inc.; identify Solid Stride Technology Partners Limited as communication hub only; use Stacey Malitowski spelling
Controls names in ARC-01
Immediate
Stacey / Noel  [row end]

Volume I approved draft
No scientific-scope change through ARC-01; add cross-reference only if formally approved through document change control
Volume I remains canonical foundation
After ARC-01 approval
Dr. Shapiro  [row end]

GOV-01 Governance and Decision Rights
Add architecture decision owners, change authority, Permit/Deny/Abstain policy ownership, Volume II gate
Implements decision rights
High
Dr. Shapiro / Stacey  [row end]

DAT-01 Data Governance and Corpus Control
Add CGE fields, source authority, anonymization verification, identity separation, provenance, retention, promotion gate
Governs all packets and feedback
High
Data owner / Dr. Shapiro  [row end]

SEC-01 Security, Privacy, and Access Control
Add trust zones, ABAC, pseudonymous IDs, cryptographic prerequisites, AI gateway, logging failure policy
Converts assumptions to controls
High
Security/institutional review  [row end]

COM-01 Research Team Operations Manual
Add approved terminology, escalation, architecture decisions, AI-use records, review and release workflow
Prevents terminology drift
Medium
Noel / Dr. Shapiro  [row end]

QUA-01 Quality and Validation Plan
Add schema, policy, provenance, negative, accessibility, and reconstruction tests; second-review decision
Verifies ARC-01
High
Dr. Shapiro  [row end]

RISK-01 Program Risk Register
Add architecture overclaim, identifier linkage, prompt injection, poisoned knowledge, stale authority, audit loss, vendor change
Tracks residual risk
High
Steering Group  [row end]

STR-01 Future Strategy
Describe SHIELD and Volume II as non-binding hypotheses contingent on Phase 1 evidence
Prevents premature commercialization claims
Medium
Stacey / Dr. Shapiro  [row end]

Volume II
Use approved terms, typed schemas, threat model, NFRs, test evidence, operations, costs, and change governance
Formal destination
Future
Assigned architecture owner

Change-control impacts
ARC-01 approval shall not silently modify existing documents. Each affected binder document should receive a controlled revision, amendment, or cross-reference with version, rationale, approver, date, and impact. Where ARC-01 remains unapproved, binder documents may cite it only as a proposal.
Naming correction
The approved sponsor surname is Stacey Malitowski. All newly generated binder documents shall use that spelling. Any earlier incorrect surname variant is an editorial defect to be corrected when the affected document is next controlled. Historical signed documents shall not be altered; the register may record the correct identity mapping.
Four-month feasibility impact
ARC-01 is feasible as a design and schema companion during the four-month term only if it does not become an additional production-build commitment. The credible minimum is one controlled terminology release, one common-envelope schema draft, one or two synthetic typed-packet examples, an IADR decision table, and traceable questions for D7 and D8. Building the full ingestion, graph, identity, resolution, composition, rendering, and cryptographic stack by 31 December would violate Volume I scope and undermine research credibility.
17  Approval, Acceptance, and Review Record
Review method
Reviewers should assess ARC-01 against five questions:
Does every term have a bounded meaning that avoids unearned claims?
Is the proposal consistent with Volume I and the four-month research scope?
Are authority, privacy, security, provenance, time, and human decision rights structurally represented?
Can requirements be verified without relying on an LLM’s judgment?
Are open choices honestly identified with owners and decision dates?
Disposition record  [row end]

Role
Name
Decision
Conditions or reference
Date / signature  [row end]

Academic Supervisor
Dr. Sidney Shapiro
Approve / Approve with conditions / Return

  [row end]

Industry Sponsor and Final Acceptance Authority
Stacey Malitowski
Approve / Approve with conditions / Return

  [row end]

Researcher
Noel Roemmele
Acknowledge / Return

  [row end]

Institutional technical, privacy, or security reviewer, if assigned
To be assigned
Concur / Conditions / Return



Approval conditions
Approval conditions shall identify the affected requirement or term, required change, evidence, responsible owner, due date, interim restriction, and closure approval. Conditions shall not be closed by changing a status label without evidence.
Version history  [row end]

Version
Date
Status
Summary  [row end]

0.1
14 August 2026
Controlled Architecture Proposal — Joint Review Draft
Corrected and reconstructed post-review architecture dictionary; added typed packets, IADR model, runtime flow, security and NFR baselines, tests, decisions, and binder integration.

Effect of approval
Approval authorizes the team to use ARC-01 terminology and boundary rules in controlled design work, synthetic schema examples, decision tables, and Volume II planning. It does not approve a vendor, authorize client-data processing, establish an identity source, accept a cryptographic design, set production service levels, or create a commitment to build every named component. Those decisions remain subject to their own authority and evidence.
Approval with conditions shall state whether the condition blocks all use, blocks a particular packet or component, or permits restricted research use. A condition that affects authorization, privacy, security, human safety, source rights, or the Phase 1 boundary is blocking unless the responsible authority states a narrower safe restriction in writing.
Review integrity record  [row end]

Review check
Required evidence
Result / reference  [row end]

Scientific alignment
Dr. Shapiro confirms consistency with Volume I research questions, D7, D8, and Phase 1 exclusions.
  [row end]

Sponsor and operational fit
Stacey Malitowski confirms legal entity, business context, decision rights, and acceptable future-strategy framing.
  [row end]

Research execution
Noel Roemmele confirms that required records, examples, tests, and escalations are operationally understandable.
  [row end]

Institutional controls
Assigned authority confirms any required privacy, security, data, procurement, ethics, or technology conditions.
  [row end]

Terminology control
Each accepted, modified, deferred, and rejected supplied proposition is traceable to Appendix B.
  [row end]

Change impact
Binder register and affected control documents have an assigned revision or explicit no-change disposition.


Post-approval review trigger
ARC-01 shall be reviewed after Volume I D7 and D8 are accepted, after any material change to OCP Profile 0.1, before real-data runtime testing, before selecting a cryptographic or identity architecture, and before Volume II approval. An incident, material security finding, new legal restriction, invalidated research finding, or model/provider change may trigger an immediate review or withdrawal.
Appendix A — Common Governed Envelope Field Dictionary  [row end]

Field
Type
Required
Meaning and rule  [row end]

envelope_type
controlled string
yes
ocp, idp, igp, hrd, aca, observation, manifest, or another registered type.  [row end]

object_id
URI or scoped identifier
yes
Stable identifier within declared tenant or namespace; no embedded secret.  [row end]

object_version
semantic or controlled version
yes
Identifies exact object revision.  [row end]

schema_id
URI or registry identifier
yes
Identifies the validation schema.  [row end]

schema_version
controlled version
yes
Exact schema version used.  [row end]

lifecycle_status
controlled string
yes
Candidate, Under Review, Validated, Approved, Effective, Superseded, Withdrawn, Archived, or Disposed.  [row end]

release_id
identifier
conditional
Required for approved or effective releases.  [row end]

compatibility_class
controlled string
conditional
Breaking, backward-compatible, metadata-only, or not applicable.  [row end]

tenant_scope
identifier
yes
Organizational or data-domain scope in which the object is valid.  [row end]

owner_role
role reference
yes
Accountable owner function.  [row end]

steward_id
scoped actor reference
yes
Operational steward.  [row end]

created_by
agent reference
yes
Human or system agent that created the record.  [row end]

reviewed_by
agent reference array
conditional
Required for validated status.  [row end]

approved_by
agent and authority reference
conditional
Required for approved or effective status.  [row end]

approval_record
record reference
conditional
Decision, conditions, date, and authority evidence.  [row end]

created_at
UTC timestamp
yes
Record-creation time.  [row end]

observed_at
timestamp or interval
conditional
Time the underlying event or fact was observed.  [row end]

valid_from
timestamp
conditional
Beginning of real-world applicability.  [row end]

valid_to
timestamp
conditional
End of real-world applicability.  [row end]

effective_at
UTC timestamp
conditional
Time approved object becomes usable.  [row end]

expires_at
UTC timestamp
conditional
Time the object shall no longer be relied upon without refresh.  [row end]

superseded_at
UTC timestamp
conditional
Time replaced by another release.  [row end]

original_time_zone
IANA zone or offset
conditional
Retained where local time affects meaning.  [row end]

sensitivity
controlled classification
yes
Approved data classification.  [row end]

purpose
controlled string or reference
yes
Permitted processing or operational purpose.  [row end]

jurisdiction
controlled array
conditional
Legal or policy jurisdiction where applicable.  [row end]

permitted_uses
controlled array
yes
Uses explicitly allowed.  [row end]

prohibited_uses
controlled array
yes
Uses explicitly disallowed.  [row end]

disclosure_rule
policy reference
yes
Who may receive which fields and under what conditions.  [row end]

source_refs
evidence references
yes
One or more source or synthetic-origin references.  [row end]

derivation_activity
provenance reference
conditional
Transformation, model, rule, or human activity producing the object.  [row end]

evidence_quality
structured assessment
yes
Completeness, authority, freshness, confidence, and limitations.  [row end]

conflict_set
assertion references
conditional
Competing claims that must remain visible.  [row end]

canonicalization_profile
identifier
conditional
Exact canonical byte procedure where integrity operations require it.  [row end]

digest_algorithm
controlled string
conditional
Named algorithm and profile.  [row end]

digest_value
encoded bytes
conditional
Digest over declared canonical content.  [row end]

signature_ref
cryptographic record reference
conditional
Signature, certificate or key identifier, algorithm, and verification status.  [row end]

timestamp_ref
trusted-time record reference
conditional
Time-evidence record and verification status.  [row end]

structural_validation
result object
yes
Schema, suite version, date, result, defects.  [row end]

semantic_validation
result object
conditional
Reviewer, method, date, result, limitations.  [row end]

policy_validation
result object
conditional
Policy checks applicable to release or use.  [row end]

supersedes
object reference array
conditional
Earlier objects replaced prospectively.  [row end]

derived_from
object or evidence references
conditional
Direct lineage relationship.  [row end]

depends_on
object or service references
conditional
Required conditions or resources.  [row end]

related_events
event references
conditional
Events creating, using, correcting, or withdrawing the object.  [row end]

retention_schedule
schedule reference
yes
Approved record-class retention and review.  [row end]

legal_hold
boolean and reference
yes
Whether disposition is suspended and why.  [row end]

disposition_status
controlled string
yes
Retain, Archive, Eligible for Disposal, Disposed, or Hold.  [row end]

audit_ref
audit-stream reference
yes
Location or identifier for lifecycle evidence.

Appendix B — Supplied Proposition Disposition Crosswalk  [row end]

Supplied proposition
Assessment
ARC-01 disposition
Reason  [row end]

IADR governs every system action
Relevant but overbroad
Adopt as proposed decision model for governed actions
Scope, precedence, inputs, outputs, and tests were missing.  [row end]

Shield CPU performs a mathematical 64-node Lock
Unsupported
Replace with IADR policy service and 16×4 conformance matrix
Counting coverage cells is not mathematics, cryptography, or verification proof.  [row end]

Human First means consequential decisions belong exclusively to humans
Strong principle requiring nuance
Adopt with meaningful-human-control criteria
Some low-impact automation may later be authorized; a click alone is not meaningful control.  [row end]

Every object has the exact same 16 sections
Poor fit and high integration risk
Reject; use CGE plus typed payloads
OCP, identity, presentation rules, and event evidence have different semantics and risk.  [row end]

OCP contains operational truth
Misleading
Replace with versioned evidence-backed representation
Authority, evidence, conflict, time, and correction must remain explicit.  [row end]

IDP houses Authority and uses hidden Luma ID
Partly useful
Adopt typed IDP; redefine Luma ID as scoped pseudonymous rotatable ID
“Hidden” is not a control and the packet alone does not create authority.  [row end]

IGP is the declarative interface rule set
Good fit
Adopt
Must be separated from the runtime manifest.  [row end]

HRD closes every event and is cryptographically bound
Overbroad and unproven
Restrict to consequential resolution; tamper-evident until crypto verified
Not every interaction requires a decision record; cryptographic system is unspecified.  [row end]

Wisdom OCM becomes a permanent OCP after validation
Terminology and lifecycle defect
Replace with Candidate Operational Observation and governed promotion
“Wisdom” is not testable; approved objects need correction, expiry, and withdrawal.  [row end]

Analytical OCP contains pre-computed statistics and risk
Useful need, wrong type
Create Analytical Context Artifact
Derived analytics need denominator, method, uncertainty, validation, and expiry.  [row end]

OKG is the database structural core
Plausible pattern
Adopt as logical knowledge representation, not mandatory physical database
Storage technology and graph suitability require evidence and engineering decisions.  [row end]

Liquid Data is Azure graph/NoSQL with sub-100 ms edge retrieval
Premature technology and performance claim
Retain technology-neutral pattern; benchmark later
Product, region, topology, consistency, and workload are undecided.  [row end]

OneDrive/SharePoint are raw blob storage only
Possible deployment rule, not universal
Defer to data architecture decision
Institutional tools, records controls, search needs, and approved stack are not yet finalized.  [row end]

BYO-LLM makes the system model-agnostic
Materially incomplete
Replace with allow-listed model configurations and regression tests
Providers are not interchangeable and data, model, version, region, retention, and behavior matter.  [row end]

CRE intersects IDP and OCP; conflict means Abstention
Directionally correct but incomplete
Adopt tri-state IADR evaluation with policy, state, time, and dependencies
Equality or intersection is insufficient for authorization and conflict handling.  [row end]

ECE wraps CRE output in IGP
Mostly correct
ECE applies IGP and creates a manifest
Rule set and runtime instance must be distinct.  [row end]

Semantic Experience Manifest is the IGP in action
Informally useful
Define as versioned runtime instance
Must contain exact evidence, actions, accessibility, and expiry.  [row end]

Universal kernel renders five primitives
Hypothesis
Retain provisional kernel and four primitives; AOB is composite
Universality is unproven and AOB is not a peer primitive.  [row end]

Core always requires HRD
Incorrect
Core may inform or request action; HRD only for consequential decisions
Avoids approval theatre and excessive decision records.  [row end]

HRD automatically causes Wisdom/Analytical OCP
Unsafe feedback shortcut
Route event evidence into candidate review
Prevents circular validation, poisoning, and silent knowledge change.

Appendix C — Worked Field Scenario
Scenario
A field worker uses an approved mobile client to request the current procedure for accessing a relocated lockbox at an active site. The request may be spoken, but voice is only the input channel. The scenario is synthetic and demonstrates architecture behavior; it is not evidence that the system exists or that lockbox access is an approved project use case.
Initial conditions
OCP-LOCKBOX-014 v1.3 is effective and states the approved access sequence and site dependency.
A candidate observation reports that the lockbox may have moved, but the observation has not been verified.
The worker’s IDP shows current site assignment and training but the required site-specific credential status cannot be refreshed because the identity source is unavailable.
Policy requires current credential evidence for access instructions that reveal a sensitive location.
Runtime result
The gateway records request REQ-20418 and derives candidate intent retrieve_sensitive_access_procedure for SITE-17.
The CRE retrieves the effective OCP, IDP attributes, policy POL-ACCESS-09, the candidate observation, system status, and exact versions.
Intent is valid. Authority cannot be confirmed at the required freshness. Dependencies also contain an unresolved candidate relocation observation.
The IADR result is Abstain, with AUT-ATTRIBUTE-STALE and DEP-CONFLICT.
The ECE applies the Abstain IGP. The manifest directs the renderer to show that access instructions cannot be disclosed, the credential source is unavailable, and the lockbox location has an unresolved update.
The AOB Core offers two permitted choices: contact the authorized site supervisor or retry credential verification. A Pad shows non-sensitive safety context and the evidence status. No location is displayed.
If the worker chooses “contact supervisor,” that routing choice is logged. It does not create an approval HRD because no access decision was made.
An authorized supervisor later verifies the credential and adjudicates the relocation observation. If the supervisor authorizes disclosure or approves a corrected location, the consequential decision creates an HRD linked to the exact evidence and policy.
The verified relocation does not overwrite OCP v1.3. A candidate OCP v1.4 enters review, passes provenance and semantic checks, receives approval, becomes effective, and supersedes v1.3.
Why this outcome is correct
The original seven-step sequence would likely have treated IDP/OCP matching as sufficient and could have rendered stale or disputed location data. The corrected sequence distinguishes a candidate observation from approved context, treats unavailable credential freshness as a reason to abstain, prevents disclosure, records recourse, and preserves a controlled correction trail.
Control evidence produced  [row end]

Evidence item
Purpose  [row end]

Request and event record
Preserves the original channel, normalized intent, target, time, environment, and component versions.  [row end]

IADR decision object
Records Abstain, both reason codes, exact policy and packet versions, required recourse, and expiry.  [row end]

Abstain manifest
Demonstrates that sensitive location content was withheld while permitted safety context and escalation were shown.  [row end]

Interaction evidence
Records the options presented and the worker’s chosen recourse without misclassifying navigation as approval.  [row end]

Adjudication record and HRD
Shows who resolved credential and location questions, under what authority, using which evidence.  [row end]

OCP v1.4 release evidence
Preserves validation, approval, effective time, supersession of v1.3, and historical trace.

Counterfactual checks
If the credential had been current and the relocation observation absent, the same policy might have returned Permit with a short validity window.
If policy expressly prohibited disclosure to the worker’s role, the result would be Deny rather than Abstain.
If the renderer could not present the warning or escalation accessibly, composition would fail and the action would remain unavailable.
If the audit recorder were unavailable and policy required a decision record, the system would not proceed and promise to reconstruct evidence later.
If a model confidently asserted the new location without a verified source, confidence would not alter the Abstain result or promote the assertion.
Appendix D — ARC-01 Conformance Checklist
Governance and scope
[ ] Volume I remains the governing Phase 1 foundation.
[ ] ARC-01 status is shown as proposed or approved with conditions; no implied production authorization.
[ ] Legal entity is Rugged Mobile Solutions Inc.; Solid Stride Technology Partners Limited is described only in its approved communication role.
[ ] Stacey Malitowski spelling is used in new controlled documents.
[ ] Roles, approvals, and open decisions are linked to authoritative records.
Terminology
[ ] Each canonical term has one bounded definition and an explicit non-meaning.
[ ] “Mathematical Lock,” “operational truth,” “hidden identifier,” and “permanent” claims are removed or qualified.
[ ] OCP, IDP, IGP, HRD, ACA, observation, and manifest remain distinct types.
[ ] AOB is a composite envelope, not a fifth primitive.
[ ] Shield CPU and universal naming remain provisional or retired as approved.
Packets and lifecycle
[ ] Common Governed Envelope fields validate.
[ ] OCP payload preserves Volume I’s exact 16-section Profile 0.1.
[ ] IDP contains minimum necessary attributes and source/freshness evidence.
[ ] IGP remains a rule set and the manifest remains a runtime instance.
[ ] HRD materiality rules are applied and exact versions are captured.
[ ] Candidate, approval, effective, supersession, withdrawal, archive, and disposition transitions are controlled.
IADR and runtime
[ ] CRE returns Permit, Deny, or Abstain with controlled reason codes.
[ ] Policy is deterministic at the authorization boundary.
[ ] Deny and Abstain are tested separately.
[ ] Critical conflicts, stale inputs, and system failures do not default to Permit.
[ ] Renderer cannot add actions or hide mandatory evidence.
[ ] Consequential decisions are reconstructable from event evidence.
AI and knowledge promotion
[ ] Every model use is tied to an approved provider, model, version, account, region, data class, and task.
[ ] AI outputs remain proposals until review and release.
[ ] Held-out evaluation and credible baseline are preserved.
[ ] Prompt injection and source-manipulation tests are included.
[ ] Feedback loops cannot self-validate or silently promote knowledge.
Security, privacy, accessibility, and quality
[ ] Threat model and trust zones are approved for the actual deployment.
[ ] Pseudonymous identifiers are scoped, rotatable, and separable from direct identity.
[ ] Cryptographic claims identify canonicalization, algorithms, keys, time, revocation, and verification.
[ ] Data minimization, anonymization verification, retention, and deletion are documented.
[ ] User experiences meet the approved WCAG target and scenario-based human-factors tests.
[ ] Requirements trace to tests, and critical Not Tested results block release.
Appendix E — Binder Amendment and Cross-Reference Instructions
Register entry
The master binder register should add the following entry after approval:  [row end]

Field
Entry  [row end]

ID
ARC-01  [row end]

Title
SHIELD Canonical Terminology and Relational Architecture  [row end]

Version
0.1 or approved successor  [row end]

Category
Controlled Architecture Proposal  [row end]

Parent
Translation Engine Volume I v1.0  [row end]

Status
Joint Review Draft / Approved / Approved with Conditions / Returned  [row end]

Owner
Project Steering Group  [row end]

Reviewers
Dr. Sidney Shapiro; Stacey Malitowski; Noel Roemmele; assigned institutional reviewer if required  [row end]

Change record
ARC-CP-001  [row end]

Data classification
Project-controlled; no client data  [row end]

Next review
At concept disposition and after Volume I D7/D8

Cross-reference statement
Where an approved binder document needs to refer to ARC-01, use this controlled wording:
ARC-01 defines a proposed terminology and relational architecture for future schema and Volume II work. It is subordinate to Translation Engine Volume I and does not authorize production implementation, expand the four-month research scope, or convert proposed components into validated findings.
Historical record rule
Do not alter executed or signed historical artefacts to retrofit current terminology. Add a document-register mapping that identifies deprecated terms, current terms, legal entity, and effective date. Quarantined legacy sources remain discoverable for historical trace but shall not be cited as governing authority.
References
National Institute of Standards and Technology. (2014, updated 2024). NIST Special Publication 800-162: Guide to Attribute Based Access Control Definition and Considerations. Official publication page.
National Institute of Standards and Technology. (2020). NIST Special Publication 800-207: Zero Trust Architecture. Official publication page.
National Institute of Standards and Technology. (2023). Artificial Intelligence Risk Management Framework (AI RMF 1.0). Official publication page.
National Institute of Standards and Technology. (2024). Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile. Official publication page.
Rundgren, A., Jordan, B., & Erdtman, S. (2020). RFC 8785: JSON Canonicalization Scheme (JCS). RFC Editor. Official RFC.
Adams, C., Cain, P., Pinkas, D., & Zuccherato, R. (2001). RFC 3161: Internet X.509 Public Key Infrastructure Time-Stamp Protocol (TSP). RFC Editor. Official RFC.
Translation Engine Program. (2026). Translation Engine Volume I: Research Foundation, Operational Knowledge Architecture, and Four-Month Validation Program, version 1.0. Project-controlled governing research foundation.
Translation Engine Program. (2026, August 14). Translation Engine & SHIELD Architecture: Canonical Data Dictionary & Relational Map. Sponsor-supplied post-review design proposition; evaluated and dispositioned in Appendix B.
World Wide Web Consortium. (2013). PROV-O: The PROV Ontology. W3C Recommendation.
World Wide Web Consortium. (2024). Web Content Accessibility Guidelines (WCAG) 2.2. W3C Recommendation.
JSON Schema. (2022). JSON Schema Draft 2020-12. Official specification.