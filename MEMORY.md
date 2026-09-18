# MEMORY.md - long term facts for agents. No secrets here, ever.

## Voice
- Direct, plain, specific. Never hedge. Never use em dashes. No emojis in published copy.
- CTA is always join the JV OS beta at https://jaredmoss.com/jv-os, mid plus end.

## Brand
- Headlines and wordmark: Protest Guerrilla only. Carter One banned. The Last Shuriken banned for new work.
- Canvas Pure Black #000000, cards Dark Navy #0A0328, accent Electric Purple #7D12FF, body Soft Gray #D0D2D8.
- EMPIRE wordmark: vertical blend #2D0798 to #7C11FD, forward slant skewX(-12) group wrapper.

## Style anchors (ceo-substack examples)
- Park City spec draft 2026-09-08: hook in socks in glass living room, who wired the money, 5 checks, socks close.
- CEO meaning REV1 2026-09-16: suffering to beautiful state via creativity, Rich yellow envelope beat.

## Top hooks that worked
- (append one line per published draft: date, hook, saves or replies)

## Pipeline facts
- Public drafts repo: JMO-CEO/ceo-substack. Text model: google/gemini-3.5-flash-lite. Secret GEMINI_API_KEY must be exported as env GOOGLE_GENERATIVE_AI_API_KEY in the workflow, that is the exact name the Google provider reads. Zero image spend v1: code built SVG/PNG plus prompt packs.
- Cloud runbook is SOLO, one session, Task tool disabled via subagent_depth 0. Six subagent sessions exceeded 30 min on free tier (run 6 proved it). Solo run with batched tool calls and max 2 websearches fits in 30. Subagent team stays for local runs only.
- Cloud pacing law: batch independent calls per block to cut billed requests, never delegate, max 2 websearches per run, sleep 60 on 429 max twice. Free key allows about 5 requests per minute. The upstream Gemini model-turn 400 bug (opencode issues 45359, 47034, still open) strikes retried multi-session runs hardest.
- Job timeout is 30 min (6 sequential phases need it, run 5 proved 15 is too short). Minutes are free on the public repo. PR step runs on always() so partial drafts are preserved instead of vanishing.
- Daily folder: drafts/YYYY-MM-DD with article-draft.md, notes-3x.md, cover.svg, cover.png, image-prompt-pack.md, video-script-pack.md, meta.json.

## Corrections log
- 2026-09-18: Carter One banned, Protest Guerrilla locked. Last Shuriken replaced in plans and design-architect.
