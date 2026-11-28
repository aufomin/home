# Domain Docs

How the engineering skills should consume this repo's domain documentation when exploring the codebase.

## Before exploring, read these

- **`GLOSSARY-MAP.md`** at the repo root: use it to find the `GLOSSARY.md` for each case relevant to the work.
- **`cases/<case>/GLOSSARY.md`**: read the case's vocabulary before naming concepts in an issue, proposal, test, or implementation.
- **`docs/adr/`**: read ADRs that touch the area you're about to work in. Also check `cases/<case>/docs/adr/` for case-specific decisions.

If a case has no glossary or ADR yet, proceed silently. The `/domain-modeling` skill creates them when terms or decisions actually get resolved. When a new case glossary is created, add its link to `GLOSSARY-MAP.md`.

## File structure

```
/
├── GLOSSARY-MAP.md                ← links to existing case glossaries
├── docs/adr/                      ← decisions shared across cases
└── cases/
    └── <case>/
        ├── GLOSSARY.md
        └── docs/adr/              ← case-specific decisions, if any
```

## Use each case's vocabulary

When your output names a domain concept (in an issue title, a refactor proposal, a hypothesis, a test name), use the term as defined in the relevant case's `GLOSSARY.md`. For work crossing cases, read each relevant glossary and keep their terms distinct.

If the concept you need isn't in the glossary yet, reconsider whether you're inventing a term or have found a gap worth recording with `/domain-modeling`.

## Flag ADR conflicts

If your output contradicts an existing ADR, surface it explicitly rather than silently overriding:

> _Contradicts ADR-0007 (event-sourced orders), but worth reopening because…_
