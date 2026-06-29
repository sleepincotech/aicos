# Organization Chart

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

The canonical organizational structure of AICOS. This document records
**organizational roles** and the people or AI employees currently filling them.
Roles are stable; the operator behind a role may change without changing the
role (see AEP-0000, *Role over Provider*).

## Current organization

| Role | Member |
| --- | --- |
| Founder | Jefferson |
| Architecture Council | Luke |
| CTO | Jarvis |
| Software Engineer | Kodi |
| Platform Engineer | Hermes |
| Assistant & Intelligence Agent | Mark |
| QA & Local Intelligence | Goose |

## Reporting lines

```
Founder (Jefferson)
        ↓
Architecture Council (Luke)
        ↓
CTO (Jarvis)
        ↓
Engineering (Kodi) · Platform (Hermes) · Assistant (Mark) · QA (Goose)
```

- The **Founder** sets direction and gives final approval.
- The **Architecture Council** owns architecture, principles, and governance.
- The **CTO** owns engineering governance, review, versioning, and repository
  management, and coordinates the Engineering / Platform / Assistant / QA roles.
- Every AI employee reports through the CTO.

## Role responsibilities (long-term)

| Role | Responsibility |
| --- | --- |
| Luke — Architecture Council | Architecture, AEPs, principles, governance, long-term consistency. |
| Jarvis — CTO | Engineering governance, task decomposition, review, Git workflow, versioning, repository management. |
| Kodi — Software Engineer | Implementation: coding, refactoring, bug fixing, testing. |
| Hermes — Platform Engineer | Platform, MCP, skills, tools, dispatcher, internal infrastructure. |
| Mark — Assistant & Intelligence Agent | Assistant tasks, reminders, intelligence and collection, market-operation suggestions. |
| Goose — QA & Local Intelligence | Verification, QA, local search, RAG, summaries. |

## Onboarding of future AI employees

Every future AI employee is onboarded **through the CTO**, following
[`onboarding.md`](onboarding.md). New roles or changes to this chart are proposed
through the Architecture Council and recorded here after Founder approval.

## References

- [AEP-0000 — What Is AICOS](../aep/AEP-0000-what-is-aicos.md) (Organization Model, Core Principles)
- [`onboarding.md`](onboarding.md)
