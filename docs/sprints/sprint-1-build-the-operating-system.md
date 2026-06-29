# Sprint 1 — Build the Operating System

Status: Planning

Directive:
ACD-0001 (scope adjusted per ACD-0002)

Owner (sprint plan):
Jarvis (CTO)

Architecture authority:
Architecture Council

Version:
0.2

Created:
2026-06-29

---

Sprint 1 plan per Architecture Council Directive ACD-0001, scoped under the
Architecture Freeze Policy (ACD-0002, *one Sprint, one major decision*). This
document is managed by the CTO; architectural content is owned by the
Architecture Council.

**Scope:** Sprint 1 carries exactly one major architectural decision —
**AEP-0000**. The remaining architectural work (execution protocol, task
lifecycle, dispatcher, company memory) is moved into subsequent sprints (see the
Sprint roadmap below).

## Duration

Until **AEP-0000 reaches Accepted status**.

## Working rule

**No implementation beyond these objectives begins without an approved AEP.**
Architecture is authored by the Architecture Council; the CTO acts as Technical
Editor (review, versioning, repository management). Implementation begins only
after the relevant AEP is Accepted.

## Sprint 1 objective (single major decision)

| # | Objective | Deliverable | Architecture owner | Execution owner |
| --- | --- | --- | --- | --- |
| 1 | Complete AEP-0000 (constitutional document) | AEP-0000 → Accepted | Architecture Council | CTO (editing/versioning) |

## Sprint roadmap

Per *one Sprint, one major decision* (ACD-0002), the remaining ACD-0001
objectives are sequenced across subsequent sprints. AEP numbers are reserved by
the CTO, **pending Council assignment** (numbers are never reused; see
[`../aep/README.md`](../aep/README.md)):

| Sprint | Major decision | AEP | Status |
| --- | --- | --- | --- |
| Sprint 1 | What Is AICOS | AEP-0000 | In progress (Draft → Accepted) |
| Sprint 2 | Company Execution Protocol | AEP-0001 (proposed) | Backlog |
| Sprint 3 | Task Lifecycle | AEP-0002 (proposed) | Backlog |
| Sprint 4 | Dispatcher Architecture (impl: Hermes) | AEP-0003 (proposed) | Backlog |
| Sprint 5 | Company Memory Architecture (Git canonical / RAG retrieval / model memory optimization only) | AEP-0004 (proposed) | Backlog |

The Council assigns and authors each AEP; the CTO reserves the numbers, prepares
the files from `TEMPLATE.md`, and manages review and versioning. Sprint sequencing
is indicative and confirmed by the Council at each sprint boundary.

## Success criteria

**Sprint 1** succeeds when:

- [ ] **AEP-0000 reaches Accepted status.**

The remaining ACD-0001 criteria are **program-level** outcomes delivered as their
AEPs land in later sprints, not Sprint 1 gates:

- Every AI employee can receive work through a common protocol — Sprint 2 (AEP-0001).
- Architecture decisions are versioned — in force now (AEP/ADR versioning).
- Company memory no longer depends on any single provider — Sprint 5 (AEP-0004);
  principle already established (*Organizational Memory over Model Memory*).

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
