# Shield anatomy

**Source:** [Unified Canon State v3](../../sources/docs/lumacanonos-unified-canon-state-v3.md), §2, §6–9.

## Product tier

**LumaShield** is free, public, and for personal use. **Shield**
(unqualified) is the professional/business tier and up. Confirmed by
the product owner, 2026-09-07 — see
[reconciliation/2026-09-07-shield-canon-collision.md](../../reconciliation/2026-09-07-shield-canon-collision.md).
This is also why LumaShield gets its own, separately-scoped design
system ([shield-canon](https://github.com/Solid-Stride/shield-canon),
a separate repo) — it isn't required to inherit every rule that
governs the broader professional/business Shield architecture, the
same scoping already established below for the four-Pad layout.

(Note: the broader Shield/Enterprise SHIELD architecture — Volume I/II
structure, Translation Engine, Enterprise SHIELD, etc. — has moved to
the shield-canon repo. This corpus stays LumaShield-only; see
[CONTRIBUTING.md](../../CONTRIBUTING.md).)

## Structural law — scoped to LumaShield, not universal SHIELD

> Everything works in fours.

**This is a LumaShield product decision, not a universal SHIELD
architectural constraint.** A formally approved Volume II instrument
([Approval Incorporation Addendum v0.2.1](https://github.com/Solid-Stride/shield-canon/blob/88455efd4221ee9d039888f7c0bdf570a251c840/01_CONSTITUTION/sources/shield-volume-ii-approval-incorporation-addendum-v0.2.1.md),
now in shield-canon, Decision 5) explicitly states "no universal attention score or fixed
four-option model governs every Shield" — universal SHIELD leaves the
option/Pad count open per-Shield. LumaShield specifically has chosen
four, corroborated independently by the LumaPatentOS inventory and
*The Shield Universe* atlas. See
[reconciliation/2026-09-07-no-fixed-four-option-model.md](../../reconciliation/2026-09-07-no-fixed-four-option-model.md).

LumaShield's Shield is the system's primary interaction object, built
on this product-level quaternary structure:

- **Shield Frame** — the outer boundary.
- **4 Pads** — the action zones (see [glossary: Pads](../glossary.md)),
  numbered, not labeled alphabetically.
- **Shield Core** — the center; acts as the state anchor.
- **Glow State Ring** — see [glow-system.md](../decisions/0003-glow-system.md).
- **Shield Display** — a single-line context readout.

**"Pearl" is superseded.** Several sources (the
[UI/UX Review](../../sources/docs/lumashield-ui-ux-review.md), the
[Constitution outline](../../sources/docs/shield-constitution-v2-2026-07-05.pdf.meta.md),
and [SHIELD Architecture Series Vol. II Part II](https://github.com/Solid-Stride/shield-canon/blob/88455efd4221ee9d039888f7c0bdf570a251c840/01_CONSTITUTION/sources/shield-architecture-series-volume-ii-part-ii.pdf.meta.md),
now in shield-canon)
use "Pearl" for this same central-anchor role. Confirmed with the
product owner: Core/AOB is current, Pearl is old, dropped naming — see
[reconciliation/2026-09-07-core-not-pearl.md](../../reconciliation/2026-09-07-core-not-pearl.md).

## Window / Context Window — superseded

An earlier "Window" (display-only, non-action) primitive, and its
later "Context Window" rename, are both superseded per
[reconciliation/2026-09-07-core-not-pearl.md](../../reconciliation/2026-09-07-core-not-pearl.md) —
the same reconciliation that dropped "Pearl." The
"Shield = Action / Window = Context" functional split in
[interaction-doctrine.md](../decisions/0001-interaction-doctrine.md)
is affected and needs its own follow-up correction; not yet done.

## Packet model

Packets are the unit of coordination that moves through the system.
Three types are defined at the v3 snapshot:

- Presence Packets
- Coordination Packets
- Alert Packets

Packet behavior follows the system's state-based language rule (see
[interaction-doctrine.md](../decisions/0001-interaction-doctrine.md)):
packets are **emitted**, not sent; they **propagate**, not get
delivered; routing is state-based, not command-based.

**Status:** directionally and linguistically defined, not yet
schema-bound (no formal field-level structure exists yet per the
source). Don't treat "packet" as having a fixed data shape until a
schema doc is written and reconciled.

## Presence model

- Presence is expressed via a **Teal** glow (see
  [glow-system.md](../decisions/0003-glow-system.md)).
- Presence is ambient, not explicit — passive, continuous,
  non-intrusive, not a status the user actively sets.

**Status:** partial canon. The v3 source explicitly flags the identity
and presence object model as underdefined — no identity structure,
presence state transitions, or multi-user interaction rules exist yet.
