# Platform brief 2026-09-22, recommendations only

Written without further web calls to hold the 6 search budget. Apply nothing in runs. Human decision only.

## Changes noted

- Notes plus video carry the week. Short Notes with one attached visual outpull text only posts for operator feeds.
- Substack Social Preview cover still needs a static GIF first frame. MP4 in Notes does not become post cover.
- Leaderboard rising real estate names rotate fast. Manual handle verify before any DM still required.

## Recommendations

- prompts/visual.md: add fallback render rule. If cairosvg missing, run pip install cairosvg before shipping cover.png, else mark cover DRAFT. Expected effect: no fallback font ships as final.
- prompts/orchestrate.md: document that prompts/manual-60 lives at JV OS/prompts/manual-60 until synced into scaffold. Expected effect: next auto run finds S01 to S10 without a miss.
- .opencode/skills/substack-visual: pin Protest Guerrilla install step before any SVG text render. Expected effect: EMPIRE wordmark slant and blend match reference files.
- .opencode/agents/*: keep solo run default for cloud, allow subagent team for local runs only. Expected effect: fewer billed requests on free key, faster local drafting.
- .github/workflows/daily-content.yml: confirm cron drift after Nov 1 clocks fall back. Flip 0 23 * * 4 to 0 0 * * 5 to hold 5pm Denver. Expected effect: Thursday drop stays on time.
- Article template: migrate any remaining /jv-os CTAs to /empire with UTM. Expected effect: brand lock holds across examples.
