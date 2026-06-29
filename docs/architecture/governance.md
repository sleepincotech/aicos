# Architecture Governance

Status: Approved

Owner:
Architecture Council

Repository management:
Jarvis (CTO)

Version:
1.0

Created:
2026-06-29

---

The governance process for AICOS architecture, adopted by Architecture Council
Directive **ACD-0002** (Architecture Freeze Policy). As AICOS begins
implementation, architectural stability takes priority over introducing new
ideas. Future Architecture Council proposals follow this process.

## Architecture Freeze

Once an AEP enters **active implementation**, its architecture is **frozen**. No
architectural changes may be introduced unless one of the following applies:

1. Critical architectural flaw
2. Security issue
3. Founder-approved governance exception

Otherwise, all new ideas are **deferred** to the Architecture Backlog.

## Architecture Backlog

New architectural ideas must **not** interrupt the current Sprint. They are
recorded as Architecture Backlog items in
[`architecture-backlog.md`](architecture-backlog.md):

```
AB-NNNN
Title
Status
Target Sprint
```

Backlog items are reviewed **only after the current Sprint finishes**.

## One Sprint, One Major Decision

Each Sprint introduces **at most one** major architectural decision. Minor
editorial improvements remain allowed. This keeps Engineering, Platform, and QA
synchronized.

## Architecture Lifecycle

```
Proposed
  ↓
Backlog
  ↓
Approved for Sprint
  ↓
Draft
  ↓
Review
  ↓
Accepted
  ↓
Implemented
  ↓
Superseded
```

## Current Freeze — Sprint 1

**Frozen** (no changes except for the three exceptions above):

- Executive Governance Model
- Organization Structure
- Git as Single Source of Truth
- Role over Provider
- Organizational Memory over Model Memory

**Deferred** (do not implement until explicitly scheduled — see the backlog):

- AB-0001 — Company Brain
- AB-0002 — Founder Freedom Index
- AB-0003 — Knowledge Architecture Enhancements

## References

- [`architecture-backlog.md`](architecture-backlog.md)
- [AEP-0000 — What Is AICOS](../aep/AEP-0000-what-is-aicos.md)
- [`../sprints/sprint-1-build-the-operating-system.md`](../sprints/sprint-1-build-the-operating-system.md)
- [`../organization/organization-chart.md`](../organization/organization-chart.md)
