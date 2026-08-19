# Obsidian + Git Setup

## First device

1. Clone `GlimmerRat/project-kernel` to a local folder.
2. Open that folder as an Obsidian vault.
3. In Obsidian, enable Community Plugins.
4. Install **Obsidian Git**.
5. Enable the plugin.

## Recommended Obsidian Git behaviour

Use conservative automatic syncing:

- Pull on vault startup/open.
- Auto-pull periodically.
- Auto-commit and push every 15–30 minutes while Obsidian is open.
- Pull before editing after switching devices.

For ordinary human edits, generic backup commits are acceptable. For agent-authored or material project-state changes, use descriptive commits such as:

```text
project(lexkit): update next action
decision(world-watch): add decision feedback model
handoff(memory-kernel): record reusable kernel boundary
```

## Multi-device rule

The simplest conflict-avoidance rule is: **pull before editing, push when finished**. Avoid making offline changes to the same note on two devices at once.

## iPad

If Git inside Obsidian is unreliable on iPad, use Working Copy as the Git client and expose the checked-out repository folder to Obsidian. Keep GitHub `main` as the canonical shared branch.

## Agent use

A persistent agent on the Mac mini should run `git pull --rebase` before making controlled changes, then commit and push its changes with descriptive messages. Substantial or risky rewrites can use a branch; normal project-state updates can remain on `main`.
