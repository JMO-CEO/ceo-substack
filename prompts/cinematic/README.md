# Cinematic Noir 50, source library

Scope: 50 noir-fit techniques from Melies, verbatim prompts with [Subject] intact.
No rewrites. No URL credit needed in prompts. Source slugs kept for traceability.

Use:
- `00-noir-50-index.md` is the master. 50 rows, type tags, EMPIRE use.
- `10-image-bank.md` is 32 stills-first picks. Paste into comic-pack panels and image-prompt-pack.
- `20-video-bank.md` is 18 motion-first picks. Paste into video-script-pack. ONE move per video, 10s max single scene.
- Workflow fit: pairs with `prompts/manual-60/S01-S10` rotation and `prompts/visual.md` brand overlay. Verbatim goes first, brand overlay goes last.

What paraphrased EMPIRE rewrite means:
- Verbatim: exactly as Melies wrote it. Example: `Low-key lighting on [Subject], most of the frame in deep shadow...`
- EMPIRE rewrite (not in these files, you asked for verbatim only): swap [Subject] for JARED, GOLD ALLY, villain, ledger, office. Add brand lock: black #000000, navy #0A0328, purple #7D12FF, faceless hero, one spot color per character, vice ban, text ban.
- These files keep verbatim pure. The `EMPIRE use` column tells you where each fits (Mon Director solo, Tue Relator duo, Wed proof object, Thu ally, Fri takedown, video takedown) without altering text.

Director cross-check (Runway, Veo 3.1, Kling 3.0, Kapwing 77, PromptSpace 35):
- Name the move plus speed plus duration. Example: slow push-in over 6 seconds.
- One move per clip. Stacking moves causes drift.
- Separate camera motion from subject motion. Camera tracks, subject walks.
- Always name lens plus lighting source plus direction. `35mm` plus `single practical from left` beats `cinematic`.
- Always state purpose: what the move reveals.
- For image to video: image fixes look, prompt directs motion only.
- Locked-off needs explicit `static, no camera move` or models add drift.

Brand rules for final prompts, MANDATORY every paste, verbatim alone fails QC:
- Start with style line: Original high contrast black and white noir illustration, hand drawn ink style, never photorealistic. Never name Sin City or any franchise.
- Hero: faceless by design, back to camera or face in shadow, no hat, short gray hair visible. Skin, hair, hands always grayscale. Purple lives only on costume accents, never on body.
- Spot: exactly one spot color per character. JARED Electric Purple #7D12FF on coat lining only. Ally Gold #FFBD59 one accent only. Villain Toxic Green #00E676 one accessory only.
- Bans, paste exactly: No text, no words, no letters, no numbers, no watermark, no speech bubbles, no logos, no badges, no captions, no labels in corners, no gore, no profanity, no cigarettes, no cigars, no pipes, no vapes, no alcohol, no drugs, no gambling, no cards, no dice, no lighters, no vice objects, no vices of any kind. Do not render any brand text in the image, brand type is added in layout after.
- End with colors only, never brand words in the image prompt: black #000000 canvas, navy #0A0328, purple #7D12FF accents. The words EMPIRE and Protest Guerrilla stay in layout only, never in the generator prompt. Test I05 v2 passed vice and hat but Gemini rendered an EMPIRE Protest Guerrilla corner badge because LOCK named the brand.
- Trigger scrub: delete fedora, cigarette, smoke, cigar, whiskey, bar, casino, cards, gambling from Melies verbatim before pasting. Test I05 failed because fedora plus crime grammar pulled a cigarette, a lighter, and playing cards.
- Cover stays flat vector editorial, never noir. Note art is noir from comic-pack.
- Protest Guerrilla only. Carter One banned. Last Shuriken banned.
- No em dashes. No emojis. No hedging.
