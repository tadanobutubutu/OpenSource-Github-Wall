---
name: merge-contributor-profile-pr
description: Workflow command scaffold for merge-contributor-profile-pr in OpenSource-Github-Wall.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /merge-contributor-profile-pr

Use this workflow when working on **merge-contributor-profile-pr** in `OpenSource-Github-Wall`.

## Goal

Merges a pull request that adds a new contributor's JSON file to the contributors directory.

## Common Files

- `contributors/*.json`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Review the pull request containing a new contributors/*.json file.
- Merge the pull request into the main branch.

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.