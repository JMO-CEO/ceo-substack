---
description: Run the daily Substack content team for the dated folder.
agent: orchestrator
subtask: true
---

Run the daily content team via @orchestrator for date $ARGUMENTS (default today).

Steps: read AGENT.md, MEMORY.md, BOARD.md To Do Today. Delegate research, ideation, parallel creation, then edit. Output the 6-file folder drafts/$ARGUMENTS plus meta.json. Move the BOARD.md card to In Review PR when the PR is open. Never direct push to main.
