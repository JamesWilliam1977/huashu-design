---
name: bugfix-demo-html-assets
description: Workflow command scaffold for bugfix-demo-html-assets in huashu-design.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /bugfix-demo-html-assets

Use this workflow when working on **bugfix-demo-html-assets** in `huashu-design`.

## Goal

Restores or updates demo HTML files to fix issues such as missing images or incorrect content.

## Common Files

- `demos/*.html`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Identify the broken or missing asset in demo HTML files.
- Update or restore the relevant demo HTML files.
- Commit the changes with a fix message referencing the demo and issue.

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.