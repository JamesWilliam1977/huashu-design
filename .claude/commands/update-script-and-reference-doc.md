---
name: update-script-and-reference-doc
description: Workflow command scaffold for update-script-and-reference-doc in huashu-design.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /update-script-and-reference-doc

Use this workflow when working on **update-script-and-reference-doc** in `huashu-design`.

## Goal

Updates a script file and its corresponding documentation to reflect changes in implementation or API usage.

## Common Files

- `scripts/*.mjs`
- `references/*.md`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Modify the script file to implement the new logic or API.
- Update the related reference or documentation file to describe the new behavior.
- Commit both files together with a descriptive message.

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.