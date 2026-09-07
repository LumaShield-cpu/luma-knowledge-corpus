# Decision 0006: Interaction doctrine detail — laws, anti-patterns, and metrics

**Status:** draft-tier detail, not approved canon
**Source:** [SHIELD Architecture Series, Volume III: Shield Interaction Doctrine](../../sources/docs/shield-architecture-series-volume-iii.pdf.meta.md).
Self-marked "Design Doctrine Draft." Uses "Pearl" natively — corpus
text below uses "Core" per
[reconciliation/2026-09-07-core-not-pearl.md](../../reconciliation/2026-09-07-core-not-pearl.md).

This extends [decision 0001](0001-interaction-doctrine.md) with a
fuller, more precisely-argued version of the same doctrine. No
conflicts with anything already locked — strong corroboration of "One
Tap or It Fails" and "context precedes interaction" specifically,
independently restated here almost verbatim. (Two points from this
same source *did* conflict with other corpus content and were resolved
separately: the fixed four-Pad question —
[reconciliation](../../reconciliation/2026-09-07-no-fixed-four-option-model.md) —
and the Ring/Glow/Red question —
[reconciliation](../../reconciliation/2026-09-07-ring-and-glow-split-red-stays-forbidden.md).)

## The twelve design laws

1. **Respect the Individual** — honor dignity, autonomy, and cognitive
   limits.
2. **Reduce Friction Relentlessly** — friction is a cost, not neutral.
3. **Zero Cognitive Load** — *not* zero thought: it targets accumulated
   interface friction, not the necessary effort of judgment,
   professional assessment, or ethical deliberation, which must be
   preserved, not eliminated.
4. **One Tap or It Fails** — the most important action must be
   reachable in one interaction.
5. **Context Precedes Interaction** — context must be established
   before any action is offered.
6. **The User Never Navigates** — the context navigates to the human.
7. **AI Owns Complexity** — reasoning/disambiguation/retrieval belongs
   to the system, never passed to the human.
8. **Humans Retain Judgment** — the final decision in consequential
   situations stays human; AI supports, never supplants.
9. **State Must Be Visible** — invisible state is a safety failure.
10. **Relationships Remain Owned by People** — SHIELD coordinates
    relationships, never owns them.
11. **Interaction Language Remains Constant** — the grammar (Dial,
    Pads, Core, Ring, Glow, Voice) doesn't change across domain, device,
    or context.
12. **Operational Calm Is Mandatory** — de-escalate, never intensify;
    no panic design, no alarm floods.

## Grammar verbs

The grammar elements (Shield, Context Window, Dial, Pads, Core, Ring,
Glow, Voice) are its nouns; a small, fixed verb set operates on them:
**Tap** (select/activate), **Hold** (secondary options / deliberate
confirmation), **Rotate** (navigate without losing focus), **Reveal**
(preview without committing), **Confirm** (affirm with deliberate
intent), **Escalate** (route to a human expert when context is
exceeded).

## Why exactly four Pads (design rationale)

Working-memory research is cited as grounding for the four-action
limit: humans can comfortably hold/compare ~4 options without decision
quality degrading; more induces choice paralysis, fewer under-uses the
surface. Per the already-reconciled resolution, this is LumaShield's
own product-level rationale for choosing four — not evidence of a
universal SHIELD law (which Decision 5 of the Volume II addendum
explicitly rules out).

## SHIELD is not a dashboard

A dashboard displays information for interpretation; SHIELD coordinates
action with comprehension already established. The Context Window
[superseded framing, see shield-anatomy.md] may display data, but the
interaction grammar itself never asks the human to interpret raw data
into action — that's a systemic failure mode in high-stakes contexts,
not a minor inconvenience.

## Voice as operational ambassador

Voice is explicitly **not a chatbot** — it's present to accomplish
things, not to converse or perform: capture intent hands-free, clarify
ambiguity with one precise question (never a form-like sequence),
retrieve memory without navigation, coordinate services without
app-switching. Required character: calm, respectful, concise, useful,
non-intrusive — and explicitly never manipulative (no scarcity
language, urgency inflation, or emotional appeals). This is the same
"operational ambassador, not chatbot" framing already captured for AI
generally in [composition-engine.md](../architecture/composition-engine.md).

## The 90–3–5 onboarding rule

An empirically-testable onboarding benchmark, particularly for
LumaShield / first-time public users:
- **90 seconds** — a new user completes at least one meaningful action
  unassisted.
- **3 minutes** — the user experiences something they understand they
  couldn't have done as efficiently without SHIELD.
- **5 minutes** — the case for returning is self-evident from the
  experience itself, not from marketing.

Testing must use genuine new users (not designers, engineers, or early
adopters) and measure objective time-to-completion. Where the rule
isn't met, the design changes — not the rule.

## Trust and privacy experience

Trust is built through **visible control**, not reassuring language or
policy documents. A user must always be able to see: what's shared,
with whom, for how long, why (in plain operational language, not
legal/technical language), and be able to revoke access immediately,
with no navigation or support contact required.

## Interaction anti-patterns

A named list of failure modes design review should check against:
Menu Sprawl, Dashboard Overload, Notification Spam, AI Impersonating
Experts (attribution must always be accurate/verifiable), Hidden
Automation (nothing executes without visible authorization), Forced
Permanent Connections (every connection needs a clean, frictionless
end), Ambiguous Core (an unclear confirmation target is a design
failure, not a minor imprecision), Excessive Pad Changes (destroys
spatial memory), Emotional Manipulation, Panic Visuals, Dark Patterns,
and Unclear State.

## Consequences

- The anti-pattern list is a ready-made design-review checklist —
  useful as-is even at draft-tier.
- The 90-3-5 Rule gives this corpus its first concrete, testable UX
  acceptance criterion; worth promoting to a harder decision once
  independently confirmed or used in actual testing.
- "AI Impersonating Experts" reinforces the Ask-Expert pattern's core
  rule (never pretend to be the expert) from a different angle —
  attribution, not just behavior.
