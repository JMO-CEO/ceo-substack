# Platform brief 2026-10-08, recommendations only

Written without further web calls to hold the 6 search budget. Apply nothing in runs. Human decision only.

## Changes noted

- Substack video uploads in Notes continue to gain organic reach when paired with single-scene motion loops.
- Subscriber growth relies heavily on direct Note engagement rather than feed browsing alone.
- Rising real estate creator lists require manual handle verification before outreach.

## Recommendations

- prompts/visual.md: add automated fallback test for cairosvg rendering during SVG-to-PNG export to ensure cover PNGs never drop to flat fallback cards without warning. Expected effect: higher fidelity visual assets across all weekly runs.
- prompts/orchestrate.md: ensure ISO week modulus calculation is documented for edge cases where ISO week numbers cross calendar years. Expected effect: zero drift in cinematic week rotation selection.
- .opencode/skills/substack-visual: pin Protest Guerrilla font verification in environment setup scripts. Expected effect: exact brand typography matching on all generated headers.
- .opencode/agents/*: maintain solo execution mode for cloud GitHub Actions to minimize rate limit exposure. Expected effect: robust execution within API constraints.
- .github/workflows/daily-content.yml: verify workflow cron schedules following daylight saving time transitions. Expected effect: prompt execution timing.
