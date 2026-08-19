---
project_id: personal-memory-kernel
name: Personal Memory Kernel
status: active
priority: now
phase: post-mvp
stage: reusable-kernel-application-integration
next_action: Define how the kernel branches into project-specific applications and project-state tracking
blocked: false
updated: 2026-08-19
notion_project_id: 3c1ab890-e487-81a9-909c-c53aa29e0809
repository: https://github.com/GlimmerRat/my-local-memory-kernel
---

## Objective

Provide a reusable local-first persistent memory primitive that can be embedded into different applications.

## Current state

Core MVP is complete and the public/local-store boundary has been established. The next design problem is reuse across multiple application contexts rather than only a personal second-brain implementation.

## Current milestone

Define the reusable kernel boundary for project control and other applications.

## Open questions

- Which project events should be promoted into memory.
- How application-specific schemas should sit above the core kernel.
- How decisions, actions, outcomes, and human reasoning should be represented.
