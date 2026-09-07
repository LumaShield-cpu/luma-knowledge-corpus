# Reconciliation: SHIELD / SHIELD Edge / Enterprise SHIELD naming and deployment model

**Date:** 2026-09-07
**Author:** Stacey (via reconciliation session)

## Conflict

Three overlapping naming questions had accumulated:

1. [shield-symantec-human-interaction-layer-domain.pdf](../sources/docs/shield-symantec-human-interaction-layer-domain.pdf.meta.md)
   and [shield-edge.pdf](../sources/docs/shield-edge.pdf.meta.md) looked
   like possible duplicates when first ingested.
2. ARCH-02 §19 names Volume II "Enterprise SHIELD — **Semantic Human
   Intelligence & Execution** Layer Domain," while both PDFs above
   self-describe as "**Symantec Human Interaction** Layer Domain" — a
   different backronym for the same S.H.I.E.L.D. initialism.
3. It wasn't clear how "SHIELD," "SHIELD Edge," and "Enterprise
   SHIELD" relate — synonyms, or different things.

## Evidence

**On (1):** a full-text diff confirms `shield-edge.pdf` is a
line-for-line match of `shield-symantec-human-interaction-layer-domain.pdf`
with every instance of "SHIELD" replaced by "SHIELD Edge" — same six
rendering layers, same seven core principles, same Core/Ring/Pads/
Dial/AOB primitives, same deployment models. This is a rename, not two
independent documents.

**On (2) and (3):** direct clarification from the product owner:
*"Shield and Enterprise Shield are installed. Shield Edge is [a]
kernel, browser-based, on device."*

## Resolution

- **`shield-edge.pdf` supersedes `shield-symantec-human-interaction-layer-domain.pdf`.**
  The older file is marked superseded in place (not deleted, per
  convention) — same content, "SHIELD Edge" is the current name.
- **The backronym is corrected**: "Semantic Human Intelligence &
  Execution Layer Domain" (ARCH-02, constitutional canon) supersedes
  "Symantec Human Interaction Layer Domain" (the informal draft
  wording both PDFs used).
- **"SHIELD," "SHIELD Edge," and "Enterprise SHIELD" are not
  synonyms** — they're different deployment forms of the same Volume
  II architecture:
  - **Shield** and **Enterprise SHIELD** are **installed** (native
    client) products.
  - **SHIELD Edge** is the **browser-based, on-device kernel** —
    matching the PDF's own "Universal Browser Rendering Kernel /
    Zero Proprietary Client" emphasis and its three deployment models
    (Connected Browser, Offline Browser, Air-Gapped Enterprise
    Appliance). It's a way of *realizing* the Volume II Composition &
    Rendering Architecture without installing a native client, not a
    fourth, separate architecture.

## Corpus update

- [corpus/architecture/enterprise-shield.md](../corpus/architecture/enterprise-shield.md) —
  new doc describing Volume II / Enterprise SHIELD and the SHIELD Edge
  deployment model, citing `shield-edge.pdf` as primary.
- `shield-symantec-human-interaction-layer-domain.pdf.meta.md` —
  marked superseded.
