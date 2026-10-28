---
name: commit-message
description: Generate a commit message that follows Conventional Commits, for a commit described by the user or the last task performed by Claude.
---

Analyze the message sent when this skill was activated and reply with a commit message that follows Conventional Commits.

The message may consist of code or a written description of a task that was performed.

If there is no message or code attached to the command, generate a commit message for the last task completed.

When generating a commit message, always follow the commit conventions of the user’s organization, if any exist.