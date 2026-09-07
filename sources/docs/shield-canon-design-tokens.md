<!--
Provenance
  Original path: 03_VISUAL_GRAMMAR/DESIGN_TOKENS.md
  Repo: github.com/Solid-Stride/shield-canon (local clone: /Users/stazz/Projects/shield-canon)
  Branch: main. HEAD at retrieval: 65cd164a01cbf455d5980d0be0d06d5ae21f52d5
  Blob SHA: 18fcb3613f4e0d94d2b9720a0fec17c07d1bbcc8
  Last commit touching this file: f92b49371b6916b2407b8c6d5d8c874b0945fcdd,
  2026-07-07 11:47:12 -0600, author "Copilot App" (machine-authored)
  Retrieved via: a peer Claude session (session local_d4c8a747-882e-4247-9a05-2964fb5a6093)
  working directly in the shield-canon repo, verbatim, at 2026-09-07.
  Working tree was clean at retrieval.

  Status: RAW, self-marked APPROVED within shield-canon's own repo, but
  shield-canon is scoped separately from the broader SHIELD Architecture
  Series (confirmed by product owner: shield-canon = LumaShield, the
  free public/personal-use product; "Shield" proper = professional/
  business tier and up). See
  /reconciliation/2026-09-07-shield-canon-collision.md for how this
  bears on the "Red is forbidden" rule reconciled elsewhere in this
  corpus.

  Note (from the retrieving session): Usage Rule 1 makes this token set
  exclusive ("must use only canonical tokens from this document") and
  Rule 2 forbids hardcoding outside it -- so #E5484D is not merely
  present, it is the only available token for both
  color.action.danger and color.state.error. There is no non-red
  alternative in this file for those semantics.
-->

# Design Tokens

This document defines canonical design tokens for visual consistency across all render targets.

## Color Tokens

| Token | Value | Usage |
|-------|-------|-------|
| color.surface.primary | #101418 | Primary background |
| color.surface.secondary | #17202A | Secondary background |
| color.text.primary | #F5F7FA | Primary text |
| color.text.secondary | #B6C2D1 | Secondary text |
| color.action.primary | #2D7FF9 | Primary actions |
| color.action.danger | #E5484D | Destructive actions |
| color.state.success | #1FA971 | Success feedback |
| color.state.error | #E5484D | Error feedback |

## Typography Tokens

| Token | Value | Usage |
|-------|-------|-------|
| font.family.base | Inter, system-ui, sans-serif | Base text |
| font.size.xs | 12px | Metadata |
| font.size.sm | 14px | Secondary text |
| font.size.md | 16px | Base text |
| font.size.lg | 20px | Section title |
| font.weight.regular | 400 | Body text |
| font.weight.medium | 500 | Emphasis |
| font.weight.bold | 700 | Key labels |

## Spacing Tokens

| Token | Value | Usage |
|-------|-------|-------|
| space.1 | 4px | Tight spacing |
| space.2 | 8px | Small spacing |
| space.3 | 12px | Standard spacing |
| space.4 | 16px | Medium spacing |
| space.6 | 24px | Large spacing |
| space.8 | 32px | Section spacing |

## Radius Tokens

| Token | Value | Usage |
|-------|-------|-------|
| radius.sm | 4px | Small controls |
| radius.md | 8px | Standard controls |
| radius.lg | 12px | Containers |

## Elevation Tokens

| Token | Value | Usage |
|-------|-------|-------|
| elevation.1 | 0 1px 2px rgba(0,0,0,0.24) | Base lift |
| elevation.2 | 0 4px 12px rgba(0,0,0,0.28) | Overlay lift |

## Usage Rules

1. Components in `05_COMPONENTS` must use only canonical tokens from this document.
2. Rendering logic in `08_RENDERING` must not hardcode visual values outside this token set.
3. Platform overrides are allowed only when mapped back to equivalent token semantics.

---

**Defined**: 2026-07-07
**Status**: APPROVED
