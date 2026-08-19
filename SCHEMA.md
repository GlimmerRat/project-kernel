# Project Kernel Schema

## Project file

Each project is identified by a stable `project_id` and has one canonical `project.md` file.

```yaml
---
project_id: lexkit
name: LexKit
status: active
priority: now
phase: architecture
stage: mvp-definition
next_action: Define initial MVP primitives
blocked: false
updated: 2026-08-19
notion_project_id: 3c1ab890-e487-8112-b3a5-f48cd44a9d9d
repository:
---
```

### Controlled values

`status`: `active`, `paused`, `incubating`, `complete`, `archived`

`priority`: `now`, `next`, `later`

`blocked`: `true` or `false`

Dates use ISO `YYYY-MM-DD`.

## Project body

Recommended headings:

- `## Objective`
- `## Current state`
- `## Current milestone`
- `## Open questions`

## Decisions

Consequential decisions live in separate files under `decisions/`.

```yaml
---
type: decision
project_id: lexkit
date: 2026-08-19
status: accepted
---
```

Recommended headings: `Decision`, `Reason`, `Alternatives`, `Consequences`.

## Handoffs

Material handoffs live under `handoffs/` with a date, project ID, source/target environment where relevant, and a short outcome/state summary.

## Future work items

If work items are mirrored locally, use stable IDs and only sync controlled operational fields with Notion: status, actor, priority, and review state. Canonical project knowledge, architecture, decisions, and history remain vault-owned.
