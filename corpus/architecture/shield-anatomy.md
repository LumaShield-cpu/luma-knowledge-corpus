# Shield anatomy

**Source:** [Unified Canon State v3](../../sources/docs/lumacanonos-unified-canon-state-v3.md), §2, §6–9.

## Structural law

> Everything works in fours.

The Shield is the system's primary interaction object, built on a fixed
quaternary structure:

- **Shield Frame** — the outer boundary.
- **4 Pads** — the action zones (see [glossary: Pads](../glossary.md)),
  numbered, not labeled alphabetically.
- **Shield Core** — the center; acts as the state anchor.
- **Glow State Ring** — see [glow-system.md](../decisions/0003-glow-system.md).
- **Shield Display** — a single-line context readout.

One unverified naming note: a separate, later source
([UI/UX Review](../../sources/docs/lumashield-ui-ux-review.md)) refers
to the center informally as "the Pearl." The v3 source does not use this
name (it says "Shield Core"). Not promoted as canon here — flagged for
a reconciliation record if the naming actually matters going forward.

## Window system (context layer)

The Window is a separate element from the Shield itself:

- **Role:** provides context only; does not initiate action.
- **Content types:** protocol preview, participant visibility, optional
  environmental context.

This maps onto the functional role split in the interaction doctrine:
**Shield = Action**, **Window = Context** (see
[interaction-doctrine.md](../decisions/0001-interaction-doctrine.md)).

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
