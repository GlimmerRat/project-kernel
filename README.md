# Project Kernel

Project Kernel is the canonical Obsidian/Git project-control vault for project state, decisions, handoffs, work history, and agent coordination.

## Role in the system

- **Obsidian + Git** — canonical project record and version history.
- **Notion** — operational dashboard and work-queue control surface.
- **Agents** — read canonical state, perform authorised work, and update operational state.
- **Memory Kernel** — later captures high-value project events, decisions, outcomes, and retrieval context.

Notion should not silently overwrite canonical reasoning or project history. Operational fields such as task status, actor, and priority may later support controlled two-way sync.

## Vault structure

```text
Projects/
  <project>/
    project.md
    decisions/
    handoffs/
    notes/
_templates/
  project-template.md
  decision-template.md
  handoff-template.md
SCHEMA.md
```

Git does not track empty folders. Create `decisions/`, `handoffs/`, and `notes/` inside a project when they are first needed.

## Normal workflow

1. Pull before editing on a new device.
2. Work normally in Obsidian.
3. Commit and push regularly using the Obsidian Git community plugin.
4. Keep `project.md` current when project state materially changes.
5. Record consequential decisions and handoffs as separate Markdown files.

For ordinary human edits, automated backup-style commits are acceptable. Agent-authored state changes should use descriptive commit messages, for example:

```text
project(lexkit): update next action
decision(world-watch): adopt decision feedback model
handoff(memory-kernel): record reusable kernel boundary
```

## Device setup

Clone this private repository and open the cloned folder as an Obsidian vault. On desktop, install the Obsidian Git community plugin and configure pull-on-start plus periodic commit/push. Device-specific workspace state is excluded by `.gitignore`.

## Canonical rule

If Notion and the vault disagree about project knowledge, architecture, decisions, or history, **the vault is authoritative**. Notion is the operational view.