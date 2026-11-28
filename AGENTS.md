## Repository

This is my Agent Kit, a shared harness for any project. The root is for reusable skills, settings, and the development pipeline; `cases/` is for case-specific decisions and glossaries.

- **Shared skills:** `.agents/skills/` contains the project-local skill copies.
- **Agent settings:** `docs/agents/` defines the issue tracker, triage labels, and domain-document conventions.
- **Current case:** `cases/process-panel/` is the working area for the process-panel case; keep its decisions and glossary there.

## Language

Write Markdown files and all content published to GitHub in English.

## Agent skills

### Writing for agents

Load the `writing-for-agents` skill before creating or editing agent-facing documents, including this file, `docs/agents/`, and project-local copies of skills under `.agents/skills/`.

### Issue tracker

Issues and specs are tracked in GitHub Issues for `aufomin/home`. See `docs/agents/issue-tracker.md`.

### Triage labels

Triage uses the default labels. See `docs/agents/triage-labels.md`.

### Domain docs

Each case has its own glossary at `cases/<case>/GLOSSARY.md`, indexed by the root `GLOSSARY-MAP.md`. See `docs/agents/domain.md`.
