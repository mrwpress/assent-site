---
name: GitHub branch workflow
description: Required GitHub workflow - branch, work, commit, PR, never merge without approval
type: feedback
---

GitHub workflow is strictly: 1) Create a branch, 2) Work and build, 3) Commit to the branch, 4) Create a PR, 5) NEVER merge a PR without explicit user approval.

**Why:** Multiple collaborators on the repo. PRs must be reviewed before merging.

**How to apply:** Always start work on a new branch off main. Commit frequently to the branch. Open a PR when work is ready for review. Never use `gh pr merge` or merge via any method unless the user explicitly says to merge.
