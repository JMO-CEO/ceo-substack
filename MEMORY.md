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
- Cloud pacing law: ONE subagent at a time, ONE tool per block, sleep 15 between phases. Free key allows about 5 requests per minute. Parallel bursts cause 429s plus interrupted streams plus the upstream Gemini model-turn 400 bug (opencode issues 45359, 47034, still open). Sequential survives, parallel dies.
- Daily folder: drafts/YYYY-MM-DD with article-draft.md, notes-3x.md, cover.svg, cover.png, image-prompt-pack.md, video-script-pack.md, meta.json.

## Corrections log
- 2026-09-18: Carter One banned, Protest Guerrilla locked. Last Shuriken replaced in plans and design-architect.
