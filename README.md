# luma-knowledge-corpus

The single source of truth for Luma, rebuilt after months of documentation and
decision drift during development. Where old docs, tickets, and code
disagree, this repo is where that gets resolved — once, on the record — so
the answer doesn't have to be re-litigated every time it comes up.

## Why this exists

Over time, docs stopped matching the product, decisions were made in chat
threads and never written down, and tickets described plans that shipped
differently (or didn't ship at all). This repo does not assume any existing
document is correct by default — including ones in here already. Everything
in `corpus/` has been checked against current reality and is safe to treat
as true today. Everything in `sources/` is a raw, unverified pull that still
needs to earn its way in.

## Structure

```
corpus/          Canonical, current-truth knowledge. Trust this.
sources/         Raw material pulled in from docs, tickets, chats, code.
                 Unverified — inputs to reconciliation, not conclusions.
reconciliation/  The record of each conflict found and how it was resolved.
```

See the README in each directory for what belongs there and how to add to it.

## Workflow, in short

1. Pull relevant material into `sources/` (don't edit it — keep it as found,
   with where it came from and when).
2. When a source conflicts with another source, with `corpus/`, or with
   actual current behavior, open a reconciliation record in
   `reconciliation/` describing the conflict and how it was settled.
3. Once resolved, write or update the canonical doc in `corpus/` and link
   back to the reconciliation record that justified it.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the detailed process.
