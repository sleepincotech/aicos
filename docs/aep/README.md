# AEPs — AICOS Evolution Proposals

An **AEP** describes a significant change to the AICOS architecture, principles,
or organization: the *why*, the *what*, and the *direction*. Authored by the
Architecture Council, reviewed by the CTO, approved by the Founder.

For point-in-time technical decisions, use an [ADR](../architecture/adr/) instead.

## Authoring a new AEP

1. Copy [`TEMPLATE.md`](TEMPLATE.md) to `AEP-NNNN-short-slug.md`.
2. Fill in the metadata header and sections.
3. Open a PR; merge only after Founder approval.

## Naming convention

```
AEP-NNNN-short-slug.md
```

- `NNNN` — zero-padded sequential number (e.g. `0000`, `0001`).
- `short-slug` — lowercase **kebab-case** summary (e.g. `what-is-aicos`).
- Numbers are **never reused.** A superseded or withdrawn AEP keeps its number;
  its `Status` is updated, the file is not renumbered or deleted.

## Index

| AEP | Title | Status |
| --- | --- | --- |
| [AEP-0000](AEP-0000-what-is-aicos.md) | What Is AICOS | Draft |
