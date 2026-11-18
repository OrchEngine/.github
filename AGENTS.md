# OrchEngine issue policy

Applies to every repository in the OrchEngine organization.

- Every issue must have exactly one type: `Feature`, `Bug`, or `Task`.
  - `Feature` — new capability or meaningful improvement.
  - `Bug` — unexpected behavior or regression.
  - `Task` — chore, docs, quality, tooling, refactor, or gate.
- Always set the type explicitly when creating or editing an issue:
  - `gh issue create --type Feature ...`
  - `gh issue edit <number> --type Task`
- Never use `feature`, `bug`, or `chore` labels for new issues; kind lives in the issue type.
- Labels describe area, priority, and phase only.
- When touching an untyped issue, set its type.

The issue forms in this repository apply org-wide by default and set the type
automatically. They only cover the GitHub UI; CLI and API callers must pass `--type`.
