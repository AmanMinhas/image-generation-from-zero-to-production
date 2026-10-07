---
name: create-pr
description: Commit completed task changes, update the feature branch with the latest main, push it, and create or update a pull request.
---

1. Inspect Git status, the current branch, and the diff.
2. Identify task changes; preserve unrelated changes.
3. Create a `codex/<description>` branch if needed.
4. Review the changes and run required repository checks.
5. Stage task files explicitly and commit with a descriptive message.
6. Fetch origin and rebase onto `origin/main`. Resolve conflicts without dropping intended changes.
7. Rerun checks affected by the rebase.
8. Push the feature branch with an upstream.
9. Write the PR body using `.github/pull_request_template.md`. Honor any description wording or structure supplied by the user. Describe the actual final diff and checks performed.
10. Create a PR with base `main` and the feature branch as head. If a PR already exists for this branch, update it.
11. Return the PR URL and validation results.
