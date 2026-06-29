# Sprint 1 — Build the Operating System

Status: Planning

Directive:
ACD-0001

Owner (sprint plan):
Jarvis (CTO)

Architecture authority:
Architecture Council

Version:
0.1

Created:
2026-06-29

---

Sprint 1 plan per Architecture Council Directive ACD-0001. This document is
managed by the CTO; architectural content is owned by the Architecture Council.

## Duration

Until **AEP-0000 reaches Accepted status**.

## Working rule

**No implementation beyond these objectives begins without an approved AEP.**
Architecture is authored by the Architecture Council; the CTO acts as Technical
Editor (review, versioning, repository management). Implementation begins only
after the relevant AEP is Accepted.

## Objectives

| # | Objective | Deliverable | Architecture owner | Execution owner |
| --- | --- | --- | --- | --- |
| 1 | Complete AEP-0000 (constitutional document) | AEP-0000 → Accepted | Architecture Council | CTO (editing/versioning) |
| 2 | Company execution protocol — every employee executes work the same way | AEP (proposed AEP-0001) | Architecture Council | CTO |
| 3 | Task lifecycle — every task has a predictable lifecycle | AEP (proposed AEP-0002) | Architecture Council | CTO |
| 4 | Dispatcher architecture | AEP (proposed AEP-0003) | Architecture Council | Hermes (implementation, post-acceptance) |
| 5 | Company memory architecture — Git canonical, RAG retrieval, model memory optimization only | AEP (proposed AEP-0004) | Architecture Council | CTO / Hermes |

## Proposed AEP roadmap

CTO repository-management proposal, **pending Council assignment** (numbers are
never reused; see [`../aep/README.md`](../aep/README.md)):

| AEP | Title | Objective |
| --- | --- | --- |
| AEP-0000 | What Is AICOS | 1 |
| AEP-0001 | Company Execution Protocol | 2 |
| AEP-0002 | Task Lifecycle | 3 |
| AEP-0003 | Dispatcher Architecture | 4 |
| AEP-0004 | Company Memory Architecture | 5 |

The Council assigns and authors each AEP; the CTO reserves the numbers, prepares
the files from `TEMPLATE.md`, and manages review and versioning.

## Success criteria (from ACD-0001)

Sprint 1 succeeds when:

- [ ] Every AI employee can receive work through a common protocol.
- [ ] Architecture decisions are versioned.
- [ ] Company memory no longer depends on any single provider.
- [ ] **AEP-0000 reaches Accepted status.**

## Sprint 0 closeout (reference)

Sprint 0 is complete (ACD-0001), tagged `sprint-0-complete`:

- Repository initialized; AEP/ADR layout, templates, naming conventions, glossary.
- Governance and Executive Governance Model v0.1 established.
- Organization documented ([`../organization/organization-chart.md`](../organization/organization-chart.md),
  [`../organization/onboarding.md`](../organization/onboarding.md)).
- Git adopted as the Single Source of Truth.
- Architecture and engineering ownership established.
- *Organizational Memory over Model Memory* principle established (AEP-0000).
- Initial onboarding completed.

## References

- [AEP-0000 — What Is AICOS](../aep/AEP-0000-what-is-aicos.md)
- [`../organization/organization-chart.md`](../organization/organization-chart.md)
- [`../aep/README.md`](../aep/README.md)
