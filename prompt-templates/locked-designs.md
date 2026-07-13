# Locked Character Designs — Canon Reference for Prompting

Living document. Every entry here is the current visual canon for that character — anything not listed as "open" is locked and must not drift between prompts. Update when a design changes; last-write wins.

---

## SAA

**Role:** SAA-9, synthesis of a vanished civilisation. Devansh's confidante, architect of the long game.

### Locked Visual Canon
- **Head:** entirely translucent turquoise-green energy — features (eyes, brow, mouth) visible as light, not flesh. Rising plume of the same turquoise-green energy above the head. No hair, no skin on the face.
- **Neck / life-support apparatus (non-negotiable, keeps her alive):** dark metal shoulder collar with concentric recessed layers, hollow open center, small internal glowing turquoise energy nodes inside the opening, port fittings along the collar rim. Shape, size, and position never change.
- **Body:** lean human-form proportions, warm natural skin tone (pale but not green), visible hands and neck below the collar.
- **Pose (canonical reference pose):** standing full-body, right hand raised palm-up in a quiet listening gesture, left hand relaxed at her side, weight even, head lowered slightly.

### RETIRED — do not include
- The small white spiral emblem that used to sit on the front-right of her collar. **Removed from canon.** Collar surface where it was is now clean dark metal.

### Outfit Variants — Locked
- **First-meeting outfit** (historical reference only — from her first canonical image): heavy austere floor-length dark charcoal robe, dusty grey trousers, simple worn light beige/grey boots. Monastic, prison-refugee register.
- **Daily/domestic outfit — practical:** softly draped charcoal-grey tunic dress to mid-calf, natural linen-wool-blend fabric with subtle weave, wide practical scoop neckline sitting beneath the collar, three-quarter draped sleeves, gathered at the natural waist with a slim woven dark cord belt. Soft slate-grey wide-legged trousers underneath. Simple worn dark charcoal soft flats.
- **Daily/domestic outfit — feminine:** single long flowing charcoal-grey dress, ankle-length, gently fitted through the torso then A-line drape from the waist down, subtly asymmetric hem gathering above the ankle. Wide softly scooped neckline. Long draped bell sleeves gathered loosely at the wrist. Slim soft cord belt at the natural waist tied in a simple knot. Linen-silk-blend fabric, matte with a subtle sheen. Simple delicate dark charcoal flats.

### Palette Rule
Turquoise is the only saturated color in any Saa image. Everything else — outfit, collar, background — stays muted. No new accent colors introduced.

### Style Reference
Two-anchor sref for humans/humanoids applies (see midjourney-template.md).

---

## DEVANSH

**Role:** Devansh Sharma, protagonist. Black Death in Andromeda, ordinary Delhi guy on Earth.

### Locked Visual Canon
- **Face:** matched to the real-life model's photograph (identity anchor). Facial structure, eye shape and spacing, nose, mouth, jawline, brow all rendered from the model photo, translated into the painterly cel-shaded illustration style.
- **Hair:** short dark spiky cut, textured, natural.
- **Body:** lean-athletic build, broad shoulder line, warm natural skin tone.
- **Eyes (default state):** warm natural brown. Only turn to full-black void when powers are active.

### Powered State — Locked
- Eyes go pitch black.
- Black liquid suspended around the body in ribbons, droplets, and puddles — the surrounding air and floor carry the phenomenon.
- Purple/violet dagger and gold/yellow floating dagger both glow as genuine light sources — purple casts cool violet glow on his hand and the nearest black droplets, gold casts warm gold glow on his left palm.
- Combat gear (see below).

### Fabric Rendering — Locked Correction
- Devansh's clothes render as **natural cloth** — proper soft fabric folds, believable drape and weight, smooth curved shadow transitions.
- **RETIRED:** faceted, triangulated, low-poly texture on any clothing item. Never appears again.

### Outfit Variants — Locked
- **Combat / powered:** long open dark coat with wide collar, black shirt underneath, brown leather belt with buckle and two sheaths, dark trousers, laced dark boots, leather forearm wrap on the right forearm. Purple dagger held loose in right hand, gold dagger floating above left palm.
- **Civilian / off-duty (default when not in powered state):** fitted black collared cotton polo t-shirt (Zara-style everyday cotton, short sleeves, soft turn-down collar, small two-button placket, body-hugging through the chest and shoulders). Beige straight-cut casual trousers in warm sand tone, clean fit, simple side pockets. Simple clean low-profile dark casual shoes. Hands relaxed inside the front trouser pockets, shoulders loose, calm neutral expression, warm brown eyes.

### Style Reference
Human anchor sref (see midjourney-template.md). Face preservation uses multi-image: real-model photograph + latest locked civilian illustration.

---

## SURI — the Music Droid

**Role:** Part of Devansh's inner-circle household on the bridge. Music droid.

### Locked Visual Canon
- **Body:** round weathered navy-blue steel speaker sphere. Scuffed white paint chipping across the lower half, streaks and staining on the navy paint, aged brass tones on all metal parts.
- **Face:** large amber-orange woven fabric speaker grille set into the front of the sphere, ringed by a brass band. Warm inner glow behind the fabric.
- **Mechanical parts:**
  - Two brass volume-dial knobs on the front — one small at the top of the sphere, one larger on the mid-body.
  - Stubby antenna rising from the top of the sphere.
  - Small brass port on the upper right of the sphere.
  - Rivets and port fittings along the lower belly.
- **Antenna pennant:** small triangular tan/off-white canvas pennant at the top of the antenna, bearing a hand-painted lazy chubby orange tabby cartoon cat with lidded half-closed bored eyes, a slack mouth, and dark cartoon outlines. Flat cartoon comic-strip style, thick outlines, minimal shading. (Garfield-adjacent register, not the character itself.)
- **Harness / strap system — Locked:** two clean tan-beige canvas straps forming a cross/X-pattern around the sphere. One strap runs vertically over the top from front to back. One strap runs horizontally around the equator. They meet at brass buckles/rings at the crossing points. Neat stitched edges, small brass rivets and buckles at intersections. Two clean tan-canvas strap ends dangle down from the bottom of the harness.
- **Pose:** floating in mid-air.

### RETIRED — do not include
- Butterflies, moths, or bees floating around the droid.
- Any flower (sunflower, marigold) tucked at the grille edge or on the body.
- The old single loose casual strap running down the left side (superseded by the X-harness above).
- Any bunched or crumpled fabric mass behind the sphere.
- Any faceted-triangle rendering on the canvas straps.

### Character Sheet — Locked
Four-view turnaround: front, side (profile), top-down, back. All at the same scale, floating at the same height, on a shared ground line. Every detail (weathering marks, patch positions, cat pennant orientation, harness crossings) must render identically across views.

### Style Reference
Droid anchor sref (bootstrapped from an earlier clean droid grid). Never uses the human anchor.

---

## Update Protocol

1. When a design changes, edit the entry here — old canon becomes RETIRED (kept in the doc as a record of what NOT to do), new canon becomes the working locked state.
2. When a new character is locked, add a new section at the bottom.
3. Every ChatGPT Images 2.0 prompt should draw its PRESERVE EXACTLY block from the character's entry here.
4. Every Midjourney prompt for a locked character should draw its silhouette/material/face description from here.
5. If canon and a working image disagree, canon wins — regenerate the image.
