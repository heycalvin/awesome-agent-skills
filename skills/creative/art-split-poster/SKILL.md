---
name: art-split-poster
description: Use when turning one or more uploaded photos into separate high-end editorial posters with a strict 3:4 vertical canvas, an exact 50/50 photo-and-paper split, a faithful photorealistic upper panel, a tiny handmade illustration below, and restrained Chinese or bilingual typography.
---

# Art Split Poster (Editorial Photo Paper Poster)

Create one independent poster per uploaded photo. Never combine multiple source photos into one collage.

## Workflow

1. Load each source with `view_image` before editing. Treat it as the edit target, not merely a style reference.
2. Use the built-in `image_gen` edit flow. Reference only the current source/poster for each call.
3. Use a structured prompt with the following invariants:
   - strict 3:4 portrait canvas;
   - a single straight horizontal boundary at the exact 50% midpoint;
   - top 50%: preserve people, identity, faces, body proportions, pose, clothing, objects, spatial relationships, lighting, texture, and photographic mood; change only subtle editorial grading and, if needed, surrounding-background crop/outpaint;
   - bottom 50%: warm off-white rough paper, visible grain/brush marks, abundant negative space, and a small centered illustration occupying about 10–20% of the lower panel;
   - illustration: recognizable subject/gesture/object reduced to delicate imperfect ink lines plus no more than four restrained flat acrylic-like colors sampled from the photo;
   - no collage, extra people, logos, watermarks, commercial cartoon styling, 3D, glossy digital finish, crayon, colored pencil, or watercolor bleed.
4. Add typography only when requested or when it improves the cover. Keep it sparse, centered or aligned to negative space, and state every character verbatim. Prefer concise copy such as "LITTLE PASSENGER" and "DAILY LIFE · 2026"; require exact, legible glyphs and no other text.
5. Inspect every result. Validate subject fidelity, exact 3:4 ratio, midpoint split, small illustration scale, ≤4-color palette, paper texture, and text spelling. If one constraint fails, make one targeted follow-up edit rather than broad restyling.
6. Save each final image under the workspace `outputs/` folder with a stable per-photo filename; preserve earlier versions with a suffix such as `-captioned` or `-v2`.

## Prompt skeleton

```text
Use case: identity-preserve. Asset type: independent editorial poster.
Input image: Image 1 is the sole edit target.
Create one strict 3:4 vertical poster with an exact 50/50 horizontal split.
Top half: preserve [recognizable subject, identity, pose, objects, setting] as authentic photography; only subtle editorial grading; never reshape the subject.
Bottom half: warm off-white handmade paper; tiny centered [subject/object] illustration; delicate imperfect ink lines; ≤4 sampled flat colors; large negative space.
Typography (verbatim): “[title]”; “[small subtitle]”. Keep it understated and legible.
Avoid: collage, extra subjects, busy decoration, 3D, glossy digital art, crayon, colored pencil, watercolor bleed, commercial cartoon, watermark.
```

## Common failure corrections

- Split is not equal: explicitly repeat “the boundary is exactly at 50% of total pixel height.”
- Illustration is too large: cap its complete footprint at 10–20% of the lower panel and demand at least 70% blank paper around it.
- Faces or bodies drift: repeat identity/pose invariants and use the original photo as the edit target.
- Typography glyphs are wrong: run a typography-only targeted edit with exact quoted text; do not regenerate the scene.
- Aspect ratio drifts: crop/rescale non-destructively to an exact 3:4 raster after visual inspection.
