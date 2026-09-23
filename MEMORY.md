# MEMORY.md - long term facts for agents. No secrets here, ever.

## Voice
- Direct, plain, specific. Never hedge. Never use em dashes. No emojis in published copy.
- CTA is always join the JV OS beta at https://jaredmoss.com/empire, mid plus end.

## Brand
- Headlines and wordmark: Protest Guerrilla only. Carter One banned. The Last Shuriken banned for new work.
- Canvas Pure Black #000000, cards Dark Navy #0A0328, accent Electric Purple #7D12FF, body Soft Gray #D0D2D8.
- EMPIRE wordmark: vertical blend #2D0798 to #7C11FD, forward slant skewX(-12) group wrapper.
- Canonical beta URL: https://jaredmoss.com/empire (old /jv-os kept only in historical drafts, host redirect covers live traffic).
- Sin City noir, Notes only: B&W photoreal base, one spot color per character. Jared hero purple #7D12FF, gold ally #FFBD59, villain green #00E676. Covers stay flat vector editorial.
- Villain roster: banker with shark loans is default, otherwise cast from the article pain (solicitor, mixer, shredder, skimmer, lockjaw). Never a named human.
- Content lock: no cigarettes, cigars, pipes, vapes, alcohol, drugs, gambling, or any vice in any panel or clip. Color placement lock: skin, hair, and hands always grayscale, purple ONLY on costume accents and objects, never on body parts. Hero face locked to jaredmoss.com/hero-photo.jpg: man near 50, short gray flecked hair combed back, trimmed salt and pepper goatee, no hat. Spec in the run drafts folder face-lock.md.

## Style anchors (ceo-substack examples)
- Park City spec draft 2026-09-08: hook in socks in glass living room, who wired the money, 5 checks, socks close.
- CEO meaning REV1 2026-09-16: suffering to beautiful state via creativity, Rich yellow envelope beat.

## Top hooks that worked
- 2026-09-22: 5am garage plus 85 year old partner, CEO as Create Execute Optimize. PUBLISHED https://jaredmoss.substack.com/p/you-cant-build-an-empire-alone-the (saves and replies pending)
- (append one line per published draft: date, hook, saves or replies)

## Pipeline facts
- Public drafts repo: JMO-CEO/ceo-substack. Text model: google/gemini-3.5-flash-lite. Secret GEMINI_API_KEY must be exported as env GOOGLE_GENERATIVE_AI_API_KEY in the workflow, that is the exact name the Google provider reads. Zero image spend v1: code built SVG/PNG plus prompt packs.
- WEEKLY cadence: Thursday 5pm Denver, cron 0 23 * * 4 (4pm MST after Nov 1 unless flipped to 0 0 * * 5). Job timeout 30 min. Minutes are free on the public repo. The opencode CLI pushes branch opencode/dispatch-* and opens the review PR itself, no backup PR step exists.
- Cloud runbook is SOLO, one session, Task tool disabled via subagent_depth 0. Solo run with batched tool calls and max 6 websearches fits in 30. Subagent team stays for local runs only.
- Cloud pacing law: batch independent calls per block to cut billed requests, never delegate, sleep 60 on 429 max twice. Free key allows about 5 requests per minute. The upstream Gemini model-turn 400 bug (opencode issues 45359, 47034, still open) strikes retried multi-session runs hardest.
- Rotation: ISO week mod 10 picks prompts/manual-60 source S01 to S10 (0 means S10). Every adapted image and video prompt ends with the brand overlay. Video is ONE 10 second single scene max, end cards built in layout.
- Weekly folder: drafts/YYYY-MM-DD with article-draft.md, note-1.md through note-5.md (Mon Director, Tue Relator, Wed Intellectual, Thu Validator, Fri Executive, link only on note-5), cover.svg, cover.png, image-prompt-pack.md with 5 sections, video-script-pack.md 10s max single scene, comic-pack.md arc plus panels, dm-pack.md drafts only, research-brief.md 3 tracks, platform-brief.md recommendations only, meta.json.
- finals/ holds only locked winners. Everything else lives in tests/archive. Finals stay clean for the PR.
- Ally lock: veteran operator in his late 50s with a bright vibrant look (Rich Giles archetype). Gold on one small accent only. Objects standard size, never oversized.
- Quality gate law: score research, article, and every prompt 1 to 5. Rewrite anything below 3 once, then ship the best and name gaps in meta.json. Off-peak runs (~2:30am Denver) with the full 60 min timeout. Quality beats speed.
- Finals folder: drafts/YYYY-MM-DD/finals holds only locked winners (panel-1-final.png etc). Every other render lives in drafts/YYYY-MM-DD/tests/archive. Finals stay clean for the PR.
- Winning image formula (proven 2026-09-22, scored 25/25, start here on all future runs): text to image only, never attach headshots to Gemini (real face transfer is refused regardless of intent). Hero faceless by design, back to camera or face in shadow. Style line is original high contrast black and white noir illustration, never name Sin City or any franchise. Partner or ally staged small and distant per the article beat. Arrow is a slender wooden archery shaft with steel tip and small glowing fletching, never a beam or bar. Full body with feet in frame plus long body shadow. Purple ONLY as thin edge glow on lining seams plus the fletching. End cards built in layout from empire-logo.png, never rendered by a video model.
- Hard ban: cloud runs never edit .opencode, skills, prompts, opencode.json, or workflows. Improvements go in platform-brief.md for human decision.

## Corrections log
- 2026-09-18: Carter One banned, Protest Guerrilla locked. Last Shuriken replaced in plans and design-architect.
- 2026-09-18: Cloud workflow must set git identity (ceo-substack-bot) and persist checkout credentials, or agent commits and PR pushes die with ident unknown and git 128. Run 7 proved the agent writes files fine.
- 2026-09-18: PIPELINE LIVE. Run 9 produced PR 1 with all 10 content files plus meta. The opencode CLI pushes branch opencode/dispatch-* and opens the review PR itself, so no backup PR step is needed or wanted. Enable Actions read-write plus PR create permission in repo settings or delivery dies.
