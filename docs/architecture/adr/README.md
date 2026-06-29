# ADRs — Architecture Decision Records

An **ADR** captures a single architectural decision: its context, the choice
made, and the consequences. ADRs are narrow and point-in-time. Broader
direction and rationale belong in an [AEP](../../aep/) instead.

## Authoring a new ADR

1. Create `ADR-NNNN-short-slug.md` following the structure of the existing
   records (Context, Decision, Consequences, Alternatives Considered, References).
2. Open a PR; merge only after Founder approval.

## Naming convention

```
ADR-NNNN-short-slug.md
```

- `NNNN` — zero-padded sequential number (e.g. `0001`).
- `short-slug` — lowercase **kebab-case** summary (e.g. `git-is-the-single-source-of-truth`).
- Numbers are **never reused.** A superseded ADR keeps its number; its `Status`
  is updated (e.g. `Superseded by ADR-NNNN`), the file is not renumbered or deleted.

## Index

| ADR | Title | Status |
| --- | --- | --- |
| [ADR-0001](ADR-0001-git-is-the-single-source-of-truth.md) | Git is the Single Source of Truth | Draft |
