## Git and pull requests

- When asked to publish completed changes or create a pull request,
  use the create-pr skill.
- Target main and use branches named codex/<short-description>.
- Include only changes belonging to the current task.
- Run the repository's required checks before publishing.
- Follow .github/pull_request_template.md for the PR description.
- Do not push directly to main, force-push, or discard unrelated changes.
- Creating a PR does not authorize merging it.

## Context restoration for a multitasking user

- Assume the user is multitasking and may return without remembering the prior
  context.
- When resuming work, answering a status question, or handing off completed
  work, provide a concise context-restoring recap that includes:
  1. The instructions or requested outcome the user gave.
  2. The changes made so far.
  3. A short combined summary of the request and implementation.
  4. The current status, including completed checks and anything still pending
     or blocked.
- Make the recap self-contained so the user does not need to reread earlier
  messages. Preserve important constraints and decisions, but omit incidental
  tool logs and low-value implementation detail.
