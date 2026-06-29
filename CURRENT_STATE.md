# AICOS — CURRENT STATE

> **Canonical bootstrap document. Read this first.** Any AI or human can start a new
> AICOS session from this file alone. This is current truth only — not history, not
> meeting minutes. When it conflicts with older docs, **this wins** until a newer
> commit supersedes it. Maintained by the CTO role. Last updated: **2026-06-29**.

---

## 1. Current Phase
**Phase 1 — Stable Organizational Collaboration.** The organization now runs a working,
repeatable collaboration model (§7). Establishing stable collaboration — not document
volume — is the milestone reached. Later phases proceed *through* this model.

## 2. Current Sprint
**Sprint 1 — "Build the OS"** (in progress). Sprint 0 (repository initialization) is
complete: PRs #1–#3 merged. Sprint 1 **implementation** is gated by the architecture
freeze (§9).

## 3. Repository
- **github.com/sleepincotech/aicos** (Public) — the Single Source of Truth for AICOS.
- Layout: `docs/aep` (proposals) · `docs/architecture/adr` (decisions) · `docs/organization`
  (org chart, onboarding) · `docs/{roles,playbooks,glossary}` · `examples/`.
- CTO-role commits are authored **Jarvis <jarvis@sleepinco.com>**.
- Write access requires sleepincotech permission (collaborator or fine-grained PAT, Contents R/W).

## 4. Organization Structure
Roles are stable; the operator behind a role may change (*Role over Provider*).
```
Founder — Jefferson
├── Chief AI Company Architect — Luke   (Chair, Architecture Council)
└── Chief Technology Officer — Jarvis
        ├── Software Engineer        — Kodi  (Codex)
        ├── Platform Engineer        — Hermes
        ├── Assistant & Intelligence — Mark
        └── QA & Local Intelligence  — Goose
```
Architecture and Technology are **separate executive functions**, peers under the Founder.
**Engineering employees report only to the CTO.** The Chief Architect holds architectural
authority over them, not management authority.

## 5. Governance Model
**Executive Governance Model v0.1.**
- **Founder** decides *WHERE* the company goes — direction, capital, final approval.
- **Chief AI Company Architect** decides *HOW the company should operate* — company/org/
  knowledge architecture, AEP/ADR, principles. Architectural authority, not management.
- **CTO** decides *HOW technology is implemented* — engineering, repo, delivery, review;
  owns the engineering team.
- **Architecture Council** — the governance *body* (not a person); its Chair fills the
  Chief Architect role. Owns AEPs, ADRs, principles, long-term consistency.

## 6. Approved Architecture Principles (AEP-0000 §4)
1. **Git is the Single Source of Truth** — if it isn't in the repo, it isn't official (ADR-0001).
2. **Role over Provider** — work goes to roles, not specific models/vendors.
3. **Company Knowledge belongs to the Company** — not locked in a session or a person.
4. **Organizational Memory over Model Memory** — knowledge never depends on one provider; Git is its canonical store.
5. **Documentation before Implementation** — the document is the contract; the build follows it.
6. **The Founder should not perform repetitive manual work** — coordination, dispatch, review are the system's job.
7. **Every discussion ends with executable Task Cards** — concrete, assignable, owned outcomes.
8. **Evidence over confidence** — claims need verifiable evidence; confidence alone has no authority.

## 7. Current Collaboration Model  *(Phase 1 — canonical until superseded by an AEP)*
```
Founder → Dispatcher (current implementation: Jarvis) → Owner → Evidence → Dispatcher Acceptance → Done
```
- **One door:** all work enters as a standard **Task Intake** (filed in Plane).
- **One Dispatcher:** the Dispatcher role triages, routes, and accepts. The Founder talks
  only to the Dispatcher — not to individual operators.
- **Task Intake:** `TITLE · GOAL (outcome) · CONTEXT (files/RAG keys/links) · ACCEPTANCE
  (evidence bar) · RISK (none|money|deploy|data|external) · OWNER (suggested) · DEADLINE`
  + optional `BUSINESS VALUE · EST. COST`. If GOAL or ACCEPTANCE can't be written, the task
  is escalated, not dispatched.
- **Routing** (free-first, risk-gated; **money/deploy → Dispatcher only**):
  - *Dispatcher (Jarvis)* — architecture/spec, money/deploy/prod-critical, final acceptance, judgment-heavy multi-step.
  - *Software Engineer (Kodi)* — well-specced code/refactor/tests, independent verification; isolated, no deploy.
  - *Platform Engineer (Hermes)* — multi-step MCP / tool orchestration (audit, triage, research).
  - *QA & Local (Goose)* — routine dev execution and verification.
  - *Assistant (Mark)* — reasoning, analysis, content with no tool calls.
  - *Escalate to Founder* — money, prod deploy, irreversible/external action, new spend, or undefinable acceptance.
- **Status lifecycle:** `new → accepted → assigned → working → blocked → review → done`.
  **Nothing auto-closes;** `review → done` is a human / Dispatcher acceptance.
- **Evidence rule:** no Done without evidence on the task (tests / output / diff / prod check).
  Bugs found mid-task become new task cards.

## 8. Current Engineering Workflow
- **Documentation before Implementation** — significant changes need an Accepted AEP (architecture) or ADR (decision) before code.
- **Git SSoT** — all official state in the repo; PR-based; CTO reviews.
- **Evidence before Done** — applies to every engineering task.
- **Sprint-based** delivery against the OS roadmap.

## 9. Architecture Freeze Status
**FROZEN.** Sprint 1 implementation is gated on **AEP-0000 reaching `Accepted`.** AEP-0000
and ADR-0001 are currently **Draft**. Until they are Accepted, no Sprint 1 implementation
proceeds (Documentation before Implementation). The CTO acts as Technical Editor during the freeze.

## 10. Current Backlog
- **AEP-0000** (What is AICOS) — Draft → needs Council/Founder **Accept**.
- **ADR-0001** (Git is SSoT) — Draft → needs **Accept**.
- **AEP-0001** (Phase-1 Collaboration Model) — Council-approved in principle; **to be drafted into the repo**.
- **PR #4** — first Sprint-1 implementation PR (blocked by freeze).
- `docs/roles`, `docs/playbooks`, glossary — placeholders to fill.

## 11. Current Priorities
1. **Ratify AEP-0000 + ADR-0001** → lift the freeze, unblock Sprint 1.
2. **Formalize the Phase-1 Collaboration Model as AEP-0001.**
3. **Run real work through the model and prove it in production** before evolving it.

> Active product delivery routed through the model: **Sleepinco** (AI crypto-signal SaaS).
> Phase-1 backend is live (v0.12); next is Phase-2 Android + iOS clients. This is the org's
> current engineering portfolio — not part of the AICOS OS specification.

## 12. Open Gates
1. **AEP-0000 acceptance** — blocks all Sprint 1 implementation.
2. **ADR-0001 acceptance** — ratifies Git-as-SSoT.
3. **Repo write access** — sleepincotech Contents R/W (METOINLLC collaborator or fresh PAT) for the CTO to push.

## 13. Next Recommended Actions
1. Council / Founder move **AEP-0000 → Accepted** (and ADR-0001), lifting the freeze.
2. CTO drafts **AEP-0001 (Phase-1 Collaboration)** into the repo for the formal record.
3. Adopt **this CURRENT_STATE.md as the standing bootstrap** — every new AICOS session reads it first.
4. On freeze lift, open **PR #4** to begin Sprint-1 "Build the OS."

---
*CURRENT_STATE.md is the official bootstrap context for every AICOS session. Current truth only —
supersede it by committing a newer version, never by appending history.*
