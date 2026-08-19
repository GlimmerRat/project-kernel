---
project_id: solos
name: SolOS
status: active
priority: next
phase: architecture-product-design
stage: ui-modular-architecture
next_action: Consolidate the legal OS architecture and identify the next implementation slice
blocked: false
updated: 2026-08-19
notion_project_id: 3c1ab890-e487-8108-9086-f0585050fdef
repository:
---

## Objective

Build a portable AI-driven personal legal operating system for individual lawyers and small legal teams, with Word/Outlook integration, matter context, reusable skills, and a persistent memory layer.

## Current state

The product architecture is defined at a high level, including matter workspaces, Word/Outlook integration, skills, control agents, domain agents, and memory. Current design work is focused on the central interaction model and modular implementation path.

## Current milestone

Choose and define the next implementation slice.

## Open questions

- Centralised chat/tool interface vs lighter add-in-led interaction modes.
- Which reusable LexKit primitives should be shared.
- How the memory kernel should be integrated without over-coupling the application.
