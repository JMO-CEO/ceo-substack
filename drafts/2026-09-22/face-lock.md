# Hero face lock: Jared Moss

## Registered reference photos (all in jaredmoss.com)

1. hero-photo.jpg, canonical. Straight on, broad smile, dark suit, white shirt, gold tie, stone interior. Primary likeness anchor alongside No. 2.
2. hero-photo2.jpeg, likeness anchor. Straight on, plain light block wall, navy suit, white shirt, purple patterned tie, big smile. Cleanest background of the set, best for model training.
3. hero-photo.1.jpeg, casual close-up angle. Outdoor daylight, soft smile, pink shirt collar. Shows hair and goatee in natural light. Crop out the hair at the right edge before uploading.
4. hero-photo.3.jpg, three quarter profile plus torso. NYSE podium, dark suit, gold tie, looking camera right, laughing. Authority context and side angle reference for Panels 4 and 5.

Retired: hero-photo.samurai.jpeg (stylized, not a likeness source). Backup duplicate: jared-moss-hero-professional-interim-1600.jpg (same shot as canonical).

## Locked facial features (confirmed across all four)

- Man near 50, brown eyes, warm confident expression.
- Hair: medium length on top, swept back, brown with strong gray at the temples and sideburns, slightly longer at the collar in the NYSE shot.
- Goatee: trimmed salt and pepper, mustache plus chin beard, gray heaviest on the chin, closely kept in every shot.
- Strong jaw, defined chin, deep smile lines at the eyes, light forehead lines.
- No hat covering the face. Fedora from test 1B is retired. Hair stays visible in every panel.

## How to use in prompts

GEMINI: never attach headshots, never write likeness lines. Gemini refuses real face transfer regardless of intent. Hero there is faceless by design (face turned away or in shadow). See gemini-paste-pack-v3.md.

FAL.AI: attach at least two photos on every generation: hero-photo2.jpeg plus hero-photo.jpg. Add hero-photo.3.jpg for any three quarter or profile pose (Panels 4 and 5, video Clip 2). Crop hero-photo.1.jpeg square on the face before attaching. Append this line to every hero prompt:

Hero face matches the attached reference photos of Jared: man near 50, brown eyes, swept back hair brown with gray temples, trimmed salt and pepper goatee, strong jaw, no hat, likeness kept.

For video: same face, neutral determined expression, no morph between clips. Start frame of Clip 2 matches end frame of Clip 1.

## Headshot needs: filled

The requested straight on and profile coverage is done. No more photos needed for the lock. Next step is a first two photo generation test: re-run v2 1A with hero-photo2.jpeg plus hero-photo.jpg attached and score likeness on the reviewer loop rule 5.
