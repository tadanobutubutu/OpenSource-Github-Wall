---
name: add-contributor-profile
description: Workflow command scaffold for add-contributor-profile in OpenSource-Github-Wall.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /add-contributor-profile

Use this workflow when working on **add-contributor-profile** in `OpenSource-Github-Wall`.

## Goal

Adds a new contributor's profile to the project by creating a JSON file in the contributors directory.

## Common Files

- `contributors/*.json`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Create a new JSON file named after the contributor in the contributors/ directory.
- Commit the new JSON file with a message indicating the addition.
- Optionally, open a pull request for the addition.

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.