# ChatGPT Images 2.0 Editing Template — LOCKED

Master template for refining Midjourney concepts (or any reference image) using ChatGPT Images 2.0 (gpt-image-2).
Built for the workflow: **Midjourney = concept exploration → ChatGPT Images 2.0 = surgical refinement and locking.**

---

## Why ChatGPT Images 2.0 for this stage

- **~99% text rendering accuracy** — real titles, taglines, credits, labels
- **Built-in reasoning** — plans layout before drawing, follows complex multi-constraint instructions
- **Reference images act as identity anchors** — the attached image is treated as canonical
- **Up to 2K native resolution**, up to 8 images per prompt
- **Multi-aspect-ratio generation** in one call (1:1, 9:16, 16:9, 3:4)
- Follows *literal* edit instructions ("fix the left hand," "add the Order I seal to the shoulder") in a way Midjourney cannot

---

## The Master Template

```
Use the attached image as the canonical reference.

TASK: [ONE-LINE USE CASE — e.g. "Clean up and lock this character concept as production-ready reference art"]

PRESERVE EXACTLY:
- [Identity feature 1 — face, proportions, silhouette]
- [Identity feature 2 — signature outfit / material / palette]
- [Identity feature 3 — any specific marks, props, colors]
- Overall painterly cel-shaded style and matte muted palette of the reference

CHANGE / ADD / FIX:
- [Change 1]
- [Change 2]
- [Change 3]

DETAILS:
- Composition: [framing, camera distance, angle]
- Lighting: [directional and specific — e.g. "soft key light from upper left, cool rim from behind"]
- Background: [what should be behind the subject]
- Text (if any): [in quotes, with placement and typography direction]

OUTPUT:
- Aspect ratio: [1:1 / 2:3 / 3:2 / 3:4 / 16:9]
- Use case: [character reference sheet / poster / cover / portrait / turnaround / edit-in-place]
- Resolution: 2K

CONSTRAINTS:
- Do not alter [identity feature that must not drift]
- No watermarks, no extra text beyond what is specified above
```

---

## The Rules (from research, April–July 2026)

1. **Attach the reference image first, prompt second.** ChatGPT reads the image as the canonical anchor.
2. **State preservation as strictly as change.** "Keep facial features, outfit, and materials exactly as in the reference" is doing 90% of the work.
3. **Name the use case up front.** ("Character reference sheet" / "movie poster" / "book cover") — Images 2.0 calibrates polish level and layout logic to it.
4. **Lighting must be directional.** "Soft key from upper left, cool rim from behind" — not "good lighting."
5. **Any rendered text goes in quotes.** Images 2.0 renders text almost perfectly if you specify it exactly and place it explicitly ("upper third," "bottom fifth billing block").
6. **Cap negative constraints at 2–4.** More scatters the model's focus.
7. **Iterate one variable at a time.** Change lighting OR pose OR background — never all three at once, or you can't tell what made it better.
8. **Word budget: 60–150 words** for edit prompts, longer OK when adding text/complex layouts. Longer than 200 = concepts start dropping.

---

## Use-Case Presets — Fill in the Blanks

### PRESET A — Clean Up & Lock a Midjourney Concept

```
Use the attached image as the canonical reference.

TASK: Clean up and lock this character concept as production-ready reference art. Correct any anatomical or mechanical errors while keeping the design 100% intact.

PRESERVE EXACTLY:
- Face, expression, and identity of the character
- Full outfit including [materials, colors, straps, accessories]
- Overall painterly cel-shaded style and matte muted palette of the reference
- Pose and camera framing

CHANGE / ADD / FIX:
- Fix hands (correct finger count, clean geometry, natural grip)
- Fix any asymmetry in [specific area]
- Tighten line quality and remove any rendering artifacts
- Sharpen small mechanical details on [specific element]

DETAILS:
- Composition: same as reference
- Lighting: same as reference
- Background: plain warm off-white studio background, single soft ground shadow directly beneath the figure

OUTPUT:
- Aspect ratio: 3:4
- Use case: locked character reference art
- Resolution: 2K

CONSTRAINTS:
- Do not alter the character's face, proportions, or outfit
- No watermarks, no text
```

### PRESET B — Turnaround Sheet from a Single View

```
Use the attached image as the canonical reference.

TASK: Generate a character turnaround reference sheet showing this exact character from four angles: front view, three-quarter view, side profile, and back view.

PRESERVE EXACTLY:
- Face, hair/head hardware, and full identity across all four views
- Outfit including every strap, panel, prop, and color exactly as in the reference
- Overall painterly cel-shaded style and matte muted palette of the reference

CHANGE / ADD / FIX:
- Show all four angles in one image, evenly spaced left to right
- Neutral standing pose in all views (arms relaxed at sides, weight even)
- Consistent lighting across all four views

DETAILS:
- Composition: four full-body views side by side, feet aligned on a shared ground line
- Lighting: soft even studio key light, minimal shadow, no dramatic direction
- Background: plain warm off-white studio background, single soft ground shadow beneath each view

OUTPUT:
- Aspect ratio: 3:1 (wide turnaround sheet)
- Use case: production character reference sheet
- Resolution: 2K

CONSTRAINTS:
- Keep facial features, outfit, and materials identical across all four views
- No text, no labels, no watermarks
```

### PRESET C — Repose / Re-scene the Same Character

```
Use the attached image as the canonical reference.

TASK: Show this exact character in a new pose and setting for a scene illustration.

PRESERVE EXACTLY:
- Face, hair, and full identity
- Outfit, materials, colors, and every accessory from the reference
- Overall painterly cel-shaded style and matte muted palette of the reference

CHANGE / ADD / FIX:
- New pose: [describe the pose specifically — "kneeling to examine a broken piece of machinery on the ground, one hand on the debris, looking down with focused expression"]
- New setting: [describe the environment]

DETAILS:
- Composition: [framing, camera distance, angle]
- Lighting: [directional and specific]
- Background: [describe environment or leave plain]

OUTPUT:
- Aspect ratio: [choose]
- Use case: scene illustration
- Resolution: 2K

CONSTRAINTS:
- Do not alter the character's face, proportions, or outfit
- No text, no watermarks
```

### PRESET D — Add or Correct Canon Details

```
Use the attached image as the canonical reference.

TASK: Add [or correct] specific canon details on this character without changing anything else.

PRESERVE EXACTLY:
- Everything in the reference image except the elements listed below
- Overall painterly cel-shaded style and matte muted palette

CHANGE / ADD / FIX:
- Add [detail 1] on [specific location — "left shoulder pauldron"]
- Add [detail 2] on [specific location]
- Correct [detail 3 that is currently wrong or missing]

DETAILS:
- Match the rendering quality and light direction of the reference
- All added elements should look integrated, not layered on top

OUTPUT:
- Aspect ratio: same as reference
- Use case: canon-corrected reference art
- Resolution: 2K

CONSTRAINTS:
- Change nothing except the specified additions/corrections
- No text, no watermarks
```

### PRESET E — Poster / Cover with Rendered Text

```
Use the attached image as the canonical character reference.

TASK: Create a theatrical one-sheet poster using this character.

PRESERVE EXACTLY:
- Face, identity, and outfit of the character from the reference
- Overall painterly style and palette

CHANGE / ADD / FIX:
- Place the character [in the composition — "centered lower half," "off-center right," "in silhouette rising over"]
- Add environment: [describe]
- Add mood/lighting: [describe]

TEXT (render exactly as written):
- Title: "[EXACT TITLE]" in [typography direction — "bold high-tech sans-serif, quiet menace"]
- Tagline: "[exact tagline]" beneath the title in small type
- Credits: "[credits block text]" in a small billing block at the bottom fifth

DETAILS:
- Composition: upper third reserved for the title, bottom fifth reserved for credits, central area for the character and scene
- Lighting: [cinematic, specific]
- Palette: [name 2-3 colors max]

OUTPUT:
- Aspect ratio: 2:3 (theatrical one-sheet)
- Use case: theatrical one-sheet movie poster
- Resolution: 2K

CONSTRAINTS:
- Render all text exactly as written above
- Character face and outfit must match the reference exactly
- No watermarks, no additional text beyond what is quoted above
```

### PRESET F — Style Transfer (keep subject, change medium)

```
Use the attached image as the canonical reference.

TASK: Re-render this exact character in a different visual medium.

PRESERVE EXACTLY:
- Character identity: face, proportions, silhouette, outfit, accessories, palette
- Pose and framing from the reference

CHANGE:
- Visual medium: [describe target medium — "Studio Ghibli-style hand-painted watercolor," "1970s sci-fi paperback cover oil painting," "gritty ink-and-wash graphic novel panel," etc.]

DETAILS:
- Composition: same as reference
- Lighting: adapt to the target medium's conventions
- Background: [same as reference / adapted]

OUTPUT:
- Aspect ratio: 3:4
- Use case: alternate-medium concept variant
- Resolution: 2K

CONSTRAINTS:
- Character identity must remain unmistakably the same
- No text, no watermarks
```

---

## Multi-Image References (When You Have Multiple Anchors)

ChatGPT Images 2.0 accepts multiple attached images. When you attach more than one:

```
Use the attached images as canonical references:
- Image 1: [role — e.g. "character identity — face, outfit, proportions"]
- Image 2: [role — e.g. "environment reference — architecture, palette, lighting"]
- Image 3: [role — e.g. "prop reference — the specific weapon design"]

TASK: [as above]
[continue with the template]
```

Naming the role of each image is critical — otherwise the model averages them.

---

## Consistency Habits

- **Same character across many prompts** — always attach the same locked reference sheet + repeat the identity preservation clauses word-for-word.
- **When something drifts** — don't rewrite the whole prompt; just re-attach the reference and strengthen the preservation clause ("face MUST match the reference exactly").
- **When text is critical** — put it in "quotes," name the exact placement, and specify typography feel. Images 2.0 will render it accurately.
- **For posters and covers** — explicitly reserve space ("upper third for title, bottom fifth for credits") or the model fills it with subject.
- **Iterate 3-5 variations at a time** — Images 2.0 supports up to 8 per prompt; use them to A/B one variable.
