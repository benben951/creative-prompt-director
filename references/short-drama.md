# Short Drama And Video Workflow

## Route

Select the production pattern before writing prompts:

| Pattern | Use for | Default rhythm |
| --- | --- | --- |
| Vertical drama | conflict, reversal, cliffhanger | hook in 0-3s; frequent information change |
| Dialogue scene | relationship and emotional turn | reaction shots and speaking turns |
| Action scene | chase, fight, physical reveal | one dominant action per shot |
| Product commercial | desire, use, proof, packshot | product legibility before spectacle |
| Slow cinematic | mood, memory, luxury | fewer shots and longer visual holds |

## Build Continuity Bibles

Define only visible, reusable facts:

- Character: stable ID, age range, face/hair, costume layers, accessories, dominant mannerism.
- Scene: layout, entrances, landmarks, time, weather, key light direction.
- Prop/product: identity, material, color, orientation, state, owner, hand used.
- Style: realism level, palette, contrast, lens language, camera stability.
- State ledger: what changes after each shot, including position, emotion, damage, wetness, opened/closed state, and remaining objects.

Assign short stable IDs such as `C1`, `S1`, and `P1`. Repeat the relevant locked description in every standalone generation prompt; model context cannot be assumed.

## Decompose The Story

For each beat specify:

```text
Beat ID | time range | new information | emotion turn | visible action | exit hook
```

Rules:

- Make the first visible event understandable without exposition.
- Every beat must change information, emotion, power, or physical state.
- Put causally linked actions in order. Do not combine setup, impact, reaction, and aftermath in one short shot.
- Preserve geography and screen direction. If direction changes, show a neutral reorientation shot.
- Use reaction time after a reveal; do not let dialogue and emotion jump simultaneously.
- End vertical drama on a question, reversal, threat, choice, or incomplete action.

## Write Shot Cards

Use one card per generated clip:

```text
Shot ID / duration:
Purpose:
Opening state:
Visible action timeline:
Ending state:
Framing / lens / camera movement:
Character, scene, prop locks:
Dialogue / sound:
Transition in / out:
Avoid:
```

Keep the duration sum equal to the requested runtime. Reserve edit handles when clips will be cut together. For image-to-video, state exactly what comes from the reference frame and what may move.

## Compose Each English Prompt

Use this order:

```text
[format and duration]. [opening frame and locked identities].
[chronological visible action with start and end state].
[framing, lens feel, camera path, focus behavior].
[lighting, color, texture, environment motion].
[exact dialogue and sound cues, if supported].
[continuity locks and transition endpoint].
Avoid: [specific anatomy, physics, identity, continuity, text, and camera failures].
```

Do not stack incompatible camera moves. Avoid vague emotion labels alone; express emotion through gaze, breath, posture, timing, and interaction. Keep spoken lines brief enough for the shot. Do not promise lip-sync when the target model does not support it.

## Mixed Product Commercial

Carry the product ID from the product brief into every shot. Establish a clean readable product view before rapid motion. Do not let hands cover key controls or labels. End on a stable hero or packshot frame with room for separately composited copy.

## Delivery

Return a beat sheet, continuity bible, shot table, then one self-contained prompt per shot. For bilingual production, keep notes and spoken lines in Chinese while retaining an English model prompt; quote exact Chinese dialogue unchanged inside the English prompt.

