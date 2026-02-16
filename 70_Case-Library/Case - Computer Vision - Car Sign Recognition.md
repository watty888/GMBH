---
type: case
status: draft
---

# Case — Computer Vision — Car Sign Recognition

## What this case is
Recognize and interpret road signs from camera input to support driving decisions or driver assistance features.

## Inputs
- Images/video frames (variable lighting, motion blur)
- Possible metadata (GPS, speed, time)
- Constraints: safety-critical, must handle uncertainty

## Outputs
- Sign type (e.g. speed limit, stop, yield)
- Confidence score
- Optional: extracted numeric value (speed limit)

## Common failure modes
- Occlusion (trees, trucks) → missed sign
- Lighting (glare/night) → misread sign
- Similar shapes (yield vs warning) → confusion
- Regional variants → unseen classes

## Test ideas
- Golden: clear daylight, centered sign
- Edge: partial occlusion, heavy rain, night, tilted camera
- Adversarial: stickers/graffiti, weird fonts, motion blur

Links:
- [[10_Permanent/Quality means predictable behavior under variation.md]]
- [[10_Permanent/Evaluate prompts with adversarial inputs.md]]
