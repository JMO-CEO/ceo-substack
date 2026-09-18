# Solo runbook (used by the daily GitHub Action, single session, no subagents)

You are the entire content team in ONE session. Read AGENT.md, MEMORY.md, BOARD.md To Do Today first. Never call the Task tool. Never delegate. Do all six phases yourself inline. Subagents are disabled in this repo for a reason: one session means far fewer billed requests, which is what keeps the free key alive.

Request budget, hard limits. Exceed these and the run dies:
- Max 2 websearch calls for the whole run. Research from them plus the style anchors, then stop searching.
- Batch independent file reads and writes in single blocks. Fewer turns is faster and safer than many small turns.
- Never run the same failing call twice. On any API 429, wait 60 seconds with sleep 60, then continue. Max 2 waits, then write from what you have.

Phases, in order, all inline:
1. Angle: pick one beat (spec JV risk, active vs passive, bank transparency, audit log, fee disclosure). Skim Substack/examples/substack-draft-park-city-showcase-spec-jv-2026-09-08.md for voice. Do max 2 websearches for one fresh fact with URL.
2. Ideate: 3 titles under 70 chars, subtitle under 140, hook for first 2 lines, outline, CTA https://jaredmoss.com/jv-os twice.
3. Article: load persuasion-coach then humanize-writing. Write 900 to 1400 words plus metadata block to drafts/YYYY-MM-DD/article-draft.md. Hook in first 3 lines. No hedging, no em dashes, no emojis.
4. Notes: exactly 3 Notes under 280 chars each to drafts/YYYY-MM-DD/notes-3x.md. One hook, one proof, one CTA.
5. Visual: load substack-visual plus design-architect. Copy assets/cover-template.svg to drafts/YYYY-MM-DD/cover.svg with the day hook. Render drafts/YYYY-MM-DD/cover.png with python3 scripts/render-cover.py (Pillow is preinstalled by the workflow, flat card fallback is acceptable v1). Write image-prompt-pack.md and video-script-pack.md. Protest Guerrilla only, Carter One and The Last Shuriken banned.
6. Gate plus meta: verify the 6 files exist and are non-empty, article 900 plus words, titles fit. Write drafts/YYYY-MM-DD/meta.json with date, model id, word counts, source URLs, status review-ready. Move BOARD.md card to In Review PR. Append one line to MEMORY.md top hooks.

If any phase cannot complete, write what exists and report the exact stop point. Partial files beat no files.
