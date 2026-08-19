---
project_id: world-watch
name: World Watch / Specula Mundi
status: active
priority: next
phase: architecture-modelling
stage: data-assumptions-decision-feedback
next_action: Define the data-to-assumption-to-decision-to-outcome model and its memory-kernel interface
blocked: false
updated: 2026-08-19
notion_project_id: 3c1ab890-e487-81f2-942b-dc5a6d576db9
repository:
---

## Objective

Build a global monitoring and investment-research system combining slow structural data with fast live feeds, supporting explicit assumptions, portfolio decisions, outcomes, and feedback.

## Current state

The architecture is converging on a layered model of observed data, assumptions, human/model decisions, realised outcomes, and persistent memory.

## Current milestone

Define the formal data → assumptions → decisions → outcomes representation and how it interfaces with the memory kernel.

## Open questions

- Which entities and relationships belong in the slow structural graph.
- How fast/live feeds update or challenge existing assumptions.
- How human reasoning is recorded alongside model recommendations.
