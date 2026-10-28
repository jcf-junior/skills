---
name: commit-message
description: Generate a Conventional Commits message. Use when the user asks for a commit message, invokes /commit-message, or wants a change (code, diff, or task description) summarized for a commit.
---

Generate a commit message following Conventional Commits 1.0.0.
The full spec is in `reference/conventional-commits.md`; read it before writing the message.

## Input
Use, in this order:
1. Code, diff, or description provided with the request.
2. Otherwise, the last task completed in this conversation.
3. Otherwise, the staged changes (`git diff --staged`).
If none of these exist, ask the user what changed.

## Conventions
Commit conventions defined in the organization's instructions take
precedence over the spec and over anything in this skill. If the
repository has its own rules (commitlint config, CONTRIBUTING.md),
apply them as well.

## Output
Reply with only the commit message in a code block, in English.