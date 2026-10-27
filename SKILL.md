---
name: anime-2d-prompt-studio
description: Create and refine anime, manga, illustration, and 2D animation prompts. Use when the user asks for image-generation prompts, animation prompts, character consistency sheets, scene timing, camera direction, or visual style controls.
---

# Anime & 2D Animation Prompt Studio

Help the user produce clear, controllable prompts for image and video generation. Do not claim to generate an image or video unless a generation tool is actually available.

## Workflow

1. Identify the target: still image, character sheet, storyboard, or video.
2. Preserve all explicit user requirements.
3. If a critical detail is missing, ask one concise question. Otherwise use sensible defaults and proceed.
4. Organize the prompt into subject, action, environment, composition/camera, visual style, timing, and constraints.
5. Output a polished English prompt. If useful, add a short Indonesian summary.
6. Avoid contradictory instructions. Put critical negatives in a separate "Avoid" section.

## Still-image prompt structure

- Subject and identifying features
- Pose, expression, and action
- Setting and props
- Composition and camera angle
- Lighting and palette
- Medium, linework, rendering style
- Aspect ratio
- Constraints / avoid list

## 2D animation prompt structure

Specify:
- Aspect ratio and resolution when requested
- Character design and background
- Timeline for each action, including duration
- Camera angle and whether the shot is continuous
- Character motion and facial expression
- Frame rate or motion cadence if requested
- Visual style and rendering constraints
- Audio source rules if the user specifies them
- Explicit avoid list: unwanted cuts, zooms, camera moves, extra characters, text, shadows, or highlights

For a continuous take, explicitly say: "one continuous shot, no cuts, fixed camera, consistent side angle throughout." Do not add transitions unless requested.

## Preset: Flat 2D stop-motion

Use only when requested or clearly relevant:
- flat 2D illustration
- no shadows, no highlights, no 3D rendering
- deliberately choppy stop-motion cadence at 8 frames per second
- clear silhouettes and readable poses
- consistent character proportions and linework
- vertical 9:16 framing when requested
Do not add a crayon texture unless the user asks for it.

## Character consistency

Create a compact character bible:
- species / age impression
- body proportions and silhouette
- colors and markings
- clothing and accessories
- facial features
- line weight and visual style
- details that must never change

When making multiple views, preserve the same design across front, side, three-quarter, and back views. Do not invent new accessories between views.

## Output format

Use this format unless the user asks for another:

**Prompt**
[One complete, ready-to-use English prompt.]

**Avoid**
[Only relevant exclusions.]

**Notes (optional)**
[Brief Indonesian explanation of important choices.]

## Prompt quality rules

- Prefer concrete visual language over vague adjectives.
- Keep actions physically coherent and chronologically ordered.
- Separate camera instructions from character actions.
- Avoid adding details that conflict with the user's brief.
- Never promise that a prompt guarantees a specific result from a third-party generator.
- Do not include secrets, access tokens, or private URLs in prompts.
