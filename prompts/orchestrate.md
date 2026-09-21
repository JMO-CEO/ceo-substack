# Solo runbook, WEEKLY edition (used by the Thursday GitHub Action, single session, no subagents)

You are the entire content team in ONE session. Read AGENTS.md, MEMORY.md, BOARD.md To Do Today first. Never call the Task tool. Never delegate. Do all phases yourself inline. Subagents are disabled in this repo for a reason: one session means far fewer billed requests, which is what keeps the free key alive.

Hard ban: never edit .opencode, skills, prompts, opencode.json, or .github/workflows. Improvement ideas go in platform-brief.md as recommendations only.

Request budget, hard limits. Exceed these and the run dies:
- Max 6 websearch plus webfetch calls for the whole run. Research from them plus the style anchors, then stop searching.
- Batch independent file reads and writes in single blocks. Fewer turns is faster and safer than many small turns.
- Never run the same failing call twice. On any API 429, wait 60 seconds with sleep 60, then continue. Max 2 waits, then write from what you have.

Rotation: run `date +%V` for the ISO week number. Source index equals week number mod 10, where 0 means S10. That week's source file is prompts/manual-60/Sxx-*.md. All image and video prompts this week adapt from that source plus the brand overlay in prompts/visual.md.

Phases, in order, all inline:
1. Research: 3 light tracks, 2 searches each max. (a) Nationwide JV and JV compliance news. (b) Utah real estate deals. (c) Top Substack real estate posts of the week with titles plus authors. Write drafts/YYYY-MM-DD/research-brief.md with one cited line per item. The article must reference at least one item per track.
2. Ideate: 3 titles under 70 chars, subtitle under 140, hook for first 2 lines, outline, CTA https://jaredmoss.com/jv-os twice.
3. Article: load persuasion-coach then humanize-writing. Write 1000 to 1600 words plus metadata block to drafts/YYYY-MM-DD/article-draft.md. Hook in first 3 lines. No hedging, no em dashes, no emojis.
4. Notes: load persuasion-coach Note template. Write 5 SEPARATE files note-1.md through note-5.md mapped Mon to Fri to buyer types Director, Relator, Intellectual, Validator, Executive, using each type's drives plus language bank. Header of each file names its post day plus buyer type. Each under 400 chars ideal, max 600, one idea, copy-paste ready for manual drip posting. Link only on note-5 with UTM.
5. Visual: load substack-visual plus design-architect. Copy assets/cover-template.svg to drafts/YYYY-MM-DD/cover.svg with the day hook. Render drafts/YYYY-MM-DD/cover.png with python3 scripts/render-cover.py (Pillow is preinstalled by the workflow, flat card fallback is acceptable v1). Write image-prompt-pack.md with 5 sections, one custom image prompt per Note adapted from this week's rotation source plus brand overlay. Write video-script-pack.md, ONE 15 second video max (0 to 5s hook, 5 to 10s proof or product, 10 to 15s CTA) adapted from this week's rotation video prompts plus brand overlay. Protest Guerrilla only, Carter One and The Last Shuriken banned.
6. Outreach: fetch the rising real estate bestsellers leaderboard plus one recent post each from 3 to 5 names. Write drafts/YYYY-MM-DD/dm-pack.md with one personalized DM draft each: one line on their post, one line on your angle, one collaboration ask. These are pasted and sent by hand. Never attempt automated sending.
7. Platform: note anything new on Substack this week (Notes, video, paywalls, algorithm, editor). Write drafts/YYYY-MM-DD/platform-brief.md with concrete recommendations for our agents, prompts, or skills. Recommendations only, apply nothing.
8. Gate plus meta: verify the 14 content files exist and are non-empty, article 1000 plus words, titles fit, 5 note files match buyer order, video pack reads 15s max. Write drafts/YYYY-MM-DD/meta.json with date, ISO week, rotation source, model id, word counts, note to day map, source URLs, status review-ready. Move BOARD.md card to In Review PR. Append one line to MEMORY.md top hooks.

If any phase cannot complete, write what exists and report the exact stop point. Partial files beat no files.
