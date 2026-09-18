---
description: Sync BOARD.md, todowrite, and the GitHub Issue to Done after a merged draft.
agent: orchestrator
subtask: true
---

Board sync for $ARGUMENTS (date or PR number).

Steps: verify the 6 files exist in drafts/$ARGUMENTS, confirm PR merged, move BOARD.md card to Done Published with PR link plus seat effect, append one line to MEMORY.md with what worked, close the matching GitHub Issue. Report files changed plus demo link or PR URL before marking complete.
