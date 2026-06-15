---
name: Commit memory files to repo
description: All Claude memory files must be pushed to the GitHub repo so they are shared between collaborators
type: feedback
---

Always commit memory files to the repo at `.claude/memory/`. Memories are shared context between collaborators, not local-only.

**Why:** Multiple people work on this project and need the same Claude context. Local-only memories create inconsistency.

**How to apply:** When creating or updating memory files, write them to both the local path (`~/.claude/projects/.../memory/`) and the repo path (`.claude/memory/`). Include memory file changes in commits.
