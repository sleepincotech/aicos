# AEP-0000: What Is AICOS

Status: Draft

Authors:
- Jefferson (Founder)
- Luke (Architecture Council)

Technical Editor:
- Jarvis (CTO)

Approvers:
- Founder

Version:
0.3

Created:
2026-06-27

---

## Abstract

AICOS is an operating system for AI-native companies. AEP-0000 is its founding
document: it states why AICOS exists, the problem it solves, what an AI Company
Operating System is, the principles that must not change, and the boundary
between what AICOS covers and what it does not.

This document is constitutional. Later AEPs build on it; they reference the
concepts defined here rather than redefining them. It is written to remain valid
even if every AI model, vendor, or tool the company uses is replaced.

## 1. Origin

Every company already runs on an operating system. Most never name it. People,
meetings, documents, approvals, decisions, habits, accumulated experience, and
culture together form an invisible system that decides how work actually moves.

AICOS did not begin as a theory. It began inside a real company while building an
AI organization for Sleepinco.

Rather than hiring more people, the founder assigned each part of the work to an
AI operator and gave each one a role rather than a single prompt: a role
responsible for technical leadership, one for implementation, one for platform
and tooling, one for assistance and data, one for quality and local
verification. The operators were individually capable. They wrote code, answered
questions, and automated workflows.

A problem surfaced almost immediately. The work was being done, but nothing
connected it. The founder was still the one holding context, setting priorities,
reviewing output, assigning the next task, and carrying knowledge from one
operator to the next.

The company had AI workers. It did not yet have an operating system to run them.
That missing layer is AICOS.

## 2. Problem Statement

Current AI tools make individuals faster. They do not make a company autonomous.

A coding assistant accelerates a developer. A chat agent answers a question. A
workflow tool automates a fixed sequence. Each improves a task. None of them owns
the company's context, decides what matters next, or guarantees that a decision
made today is still in force tomorrow.

The result is a single, recurring failure mode: **the founder remains the
operating system.** Context, prioritization, review, task assignment, and
knowledge transfer all route through one person. Adding more capable AI does not
remove this dependency — it often increases it, because every new operator is one
more thing for the founder to coordinate.

This document names that dependency the **primary problem** AICOS exists to
solve. The objective is not a faster founder. It is a company that can run, with
the founder setting direction rather than dispatching every step.

## 3. Definition

An **AI Company Operating System** is the layer that coordinates AI and human
operators into a single, coherent company. It owns the company's roles,
knowledge, decisions, task flow, and standards of work, so that capability does
not depend on one person holding everything together.

It is defined as much by what it is *not*:

- **It is not an AI framework.** A framework is a library for building one
  application. AICOS governs how an organization operates, not how a single
  program is structured.
- **It is not a prompt library.** Prompts configure a model's behavior for a
  task. AICOS defines durable roles and responsibilities that outlive any prompt
  or model.
- **It is not workflow automation.** Automation executes a fixed sequence of
  steps. AICOS decides which work matters, who owns it, and how it is reviewed —
  the layer above any individual workflow.
- **It is not an agent platform.** An agent platform provides a runtime for
  agents to act. AICOS is the organizational layer that gives those agents roles,
  shared knowledge, and accountability, independent of which platform runs them.

In short: frameworks, prompts, workflows, and agent platforms are tools a company
*uses*. AICOS is how the company is *run*.

## 4. Core Principles

These principles are the stable core of AICOS. They are expected to hold across
changes in models, vendors, and tooling.

- **Git is the Single Source of Truth.** The authoritative state of the company's
  knowledge, decisions, and standards lives in version control. If it is not in
  the repository, it is not official. (See ADR-0001.)
- **Role over Provider.** Work is assigned to organizational roles, not to
  specific AI models or vendors. Any provider behind a role can be replaced
  without changing the organization.
- **Company Knowledge belongs to the Company.** Context, history, and decisions
  are company assets stored centrally — not locked inside an individual operator,
  a chat session, or a person's memory.
- **Organizational Memory over Model Memory.** Company knowledge must never
  depend on any single AI provider or model. Organizational memory belongs to
  AICOS; Git is its canonical implementation. A provider may be replaced at any
  time without the company losing what it knows.
- **Documentation before Implementation.** Significant changes are written down
  and agreed before they are built. The document is the contract; the
  implementation follows it.
- **The Founder should not perform repetitive manual work.** Recurring
  coordination, dispatch, and review are responsibilities of the system, not the
  founder. Founder time is for direction and judgment.
- **Every discussion ends with executable Task Cards.** A conversation is not
  finished until it produces concrete, assignable units of work with a clear
  owner and outcome.
- **Evidence over confidence.** Claims are backed by verifiable evidence. A
  confident assertion without evidence carries no authority.

## 5. Organization Model

AICOS defines a reference organization as a set of **roles**. These are
organizational responsibilities, not AI models or products. A role may be filled
by a human, an AI operator, or several operators over time; the role and its
responsibilities remain stable while the operator behind it may change.

| Role | Responsibility |
| --- | --- |
| Founder | Sets direction, owns the company, gives final approval. |
| Architecture Council | Owns architecture, principles, governance, and long-term consistency. |
| CTO | Technical leadership, engineering governance, task decomposition, and review. |
| Software Engineer | Implementation: building, refactoring, fixing, and testing. |
| Platform Engineer | Internal platform, tooling, and infrastructure that other roles depend on. |
| Assistant | Day-to-day operational support, coordination, and information handling. |
| QA | Quality, verification, and validation of work before it is accepted. |

The roles are deliberately described without naming the AI providers currently
behind them. Binding a role to a specific model would make the organization
fragile to provider change — the opposite of what AICOS is for.

## 6. Scope

AICOS covers the organizational layer of an AI-native company. In scope:

- **Architecture** — the structure and direction of the company's systems.
- **Governance** — how decisions are proposed, reviewed, and ratified.
- **Knowledge** — how company context and history are captured and retrieved.
- **Roles** — the definition and boundaries of organizational responsibilities.
- **Engineering Standards** — the shared standards for how work is built.
- **Documentation** — the durable, authoritative record of the company.
- **Task Flow** — how work is created, assigned, and tracked to completion.
- **Review** — how output is checked before it is accepted.
- **Memory** — how knowledge persists across operators and over time.
- **Agent Collaboration** — how multiple operators work together coherently.

## 7. Non-Goals

To prevent scope creep, AICOS explicitly does **not** aim to be:

- **A specific AI model, vendor, or product.** AICOS is provider-agnostic by
  design; it depends on no single model remaining available.
- **An application framework or SDK.** It does not prescribe how to build any
  individual program.
- **A general-purpose workflow or automation engine.** Specific workflows are
  tools used within AICOS, not AICOS itself.
- **A replacement for human judgment.** It removes repetitive coordination, not
  direction, accountability, or final approval.
- **A product to be sold per seat or per feature.** AICOS is how a company is
  run, not a SaaS feature set.
- **A fixed implementation.** This document defines principles and boundaries;
  concrete mechanisms are defined in later AEPs and may evolve.

## 8. Future Evolution

AICOS is expected to evolve from a coordinated organization toward an
increasingly autonomous one, at a high level:

- From a founder who coordinates manually, toward a system that coordinates
  itself under the founder's direction.
- From knowledge and decisions recorded by hand, toward knowledge that is
  captured and surfaced as a standard part of how work happens.
- From roles operated case by case, toward a defined dispatch and control layer
  that routes work to roles automatically.

These directions are intentionally stated without implementation detail.
Mechanisms — task protocols, dispatch, memory systems, and tooling — are the
subject of future AEPs that reference this document.

## References

- ADR-0001 — Git is the Single Source of Truth.
- `docs/aep/README.md` — AEP index, authoring guide, and naming convention.
- `docs/glossary/README.md` — canonical definitions of AICOS terms.

Future AEPs reference the concepts established here rather than redefining them.
