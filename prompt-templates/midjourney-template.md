# Midjourney Character Concept Template — LOCKED

Master template for all character concept exploration on Midjourney V8.1.
Locked for consistency across the entire cast — do not change frozen elements between prompts in the same series.

---

## The Master Template

```
Full-body character concept of [SUBJECT] the size of [SIZE ANCHOR],
[silhouette + primary material + finish + one wear detail],
its face [EXPLICIT face hardware — lens / grille / dial / glass / features],
[ONE signature functional feature with light],
[POSE + personality simile],
[ONE storytelling flourish], [small hand-painted white MARK],
high-detail 2D character concept illustration, painterly cel-shaded rendering with crisp graphic edges, matte muted palette with one saturated [ACCENT COLOR] accent, gear-dense believable mechanical detailing,
plain warm off-white studio background, single soft ground shadow directly beneath it
--no text, watermark, human, humanoid, human face, human head, hair, skin
--ar 3:4 --raw --stylize 150 --chaos 0 --sw 150 --v 8.1
```

---

## What Varies (bracketed slots — change per subject)

| Slot | Purpose | Example |
|---|---|---|
| `[SUBJECT]` | Identity opener + type | "a fully mechanical, non-humanoid cooking droid" / "a humanoid figure of an aged veteran" |
| `[SIZE ANCHOR]` | Scale reference | "the size of a fat kettle" / "the size of a tall man" |
| Silhouette + material + wear | Primary read at thumbnail | "rounded cast-iron sphere body in matte soot-black with heat-discolored panel edges" |
| Face hardware | The single most important visual — describe explicitly to prevent leakage from references | "its face a wide friendly oval of amber furnace-glass glowing from the coal-core inside" |
| Signature feature | One memorable functional element | "horizontal belly vents leaking warm orange light" |
| Pose + simile | Personality shorthand | "leaning eagerly forward like a pot about to boil over" |
| Storytelling flourish | Implies a life | "one tiny biscuit resting unnoticed on its crown" |
| Hand-painted mark | Personal signature detail | "a small hand-painted white flame beside the vents" |
| `[ACCENT COLOR]` | The one saturated color | "ember-orange" / "turquoise" / "cyan" |

---

## What is Frozen (never change between prompts in a series)

| Element | Value | Why |
|---|---|---|
| Opening phrase | `Full-body character concept of` | Framing consistency |
| Style block | `high-detail 2D character concept illustration, painterly cel-shaded rendering with crisp graphic edges, matte muted palette with one saturated [X] accent, gear-dense believable mechanical detailing` | The verbal style stamp — repeat verbatim every prompt |
| Staging | `plain warm off-white studio background, single soft ground shadow directly beneath it` | Uniform staging across the cast |
| `--ar 3:4` | Portrait format | Aspect ratio changes force re-composition |
| `--raw` | Off MJ's auto-beautify | Prompt tracked more literally |
| `--stylize 150` | MJ's own aesthetic dial | Enough polish, srefs and text stay in charge |
| `--chaos 0` | Grid variation off | Every grid obeys the same layout logic |
| `--sw 150` | Style-ref authority | Full style transfer from the anchors |
| `--v 8.1` | Model version | Pin the model — future versions will drift |

---

## The `--no` Block (anti-leak)

**For non-humanoid droids/objects:**
```
--no text, watermark, human, humanoid, human face, human head, hair, skin
```

**For humanoid characters (Saa, villains, etc.):**
```
--no text, watermark
```
Dropping the anatomy exclusions when the subject IS humanoid — otherwise the `--no` block fights the prompt.

---

## Style References — the Two-Anchor Workflow

Bleed happens when style-ref images contain strong subjects with faces. Solution:

**Human characters** → use the two humanoid reference images (the viking-styled figure and the trooper-styled figure). Their anatomy is a feature here, not a leak.

**Droids / mechanical / non-humanoid** → bootstrap a droid style anchor:
1. Run ONE droid prompt with **no sref**, describing the style verbally in-prompt.
2. Pick the best result from that grid — it becomes your droid anchor.
3. From then on: `--sref [that-droid-URL] --sw 150` for every droid in the household.

This gives you two style anchors — one human line, one droid line — both in the same painterly language, with no bleed possible.

---

## Consistency Habits

- **Do not use `--p` (personalization)** in this series. If your profile evolves, your cast drifts with it.
- **Reroll rather than rewrite.** Editing words re-randomizes more than rerolling the same prompt does.
- **Draft mode (⚡) for exploration only.** Re-render keepers at full quality.
- **Match `--ar` to reference `--ar`** where possible. A 9:16 reference forced into 21:9 makes the model hallucinate.
- **For frame-exact reproducibility** (A/B tests): add `--seed [number]` temporarily; drop it for real generations.

---

## Example — Fully Filled Template (Laddu, the Hearth Cook)

```
Full-body character concept of a fully mechanical, non-humanoid cooking droid the size of a fat kettle,
rounded cast-iron sphere body in matte soot-black with heat-discolored panel edges and rivets polished bright from handling,
its face a wide friendly oval of amber furnace-glass glowing from the live coal-core inside,
horizontal belly vents leaking warm orange light onto stubby piston legs,
two padded oven-mitt hands and two folded-back brass burner arms tucked like wings,
a dented copper ladle magnetized to its hip and a tea-towel knotted through one shoulder joint,
leaning eagerly forward like a pot about to boil over,
one tiny biscuit resting unnoticed on its crown,
a small hand-painted white flame beside the vents,
high-detail 2D character concept illustration, painterly cel-shaded rendering with crisp graphic edges, matte muted palette with one saturated ember-orange accent, gear-dense believable mechanical detailing,
plain warm off-white studio background, single soft ground shadow directly beneath it
--no text, watermark, human, humanoid, human face, human head, hair, skin
--ar 3:4 --raw --stylize 150 --chaos 0 --sw 150 --v 8.1
```

---

## Adaptations by Subject Type

| Subject Type | Opening | `--no` block | Style-ref anchor |
|---|---|---|---|
| Droid / machine | `a fully mechanical, non-humanoid [type]` | full anatomy exclusion | droid anchor |
| Humanoid (human/near-human) | `a humanoid figure of [description]` | text, watermark only | human anchor (viking + trooper) |
| Insectoid / alien creature | `a [size] insectoid figure` / `an alien creature of [type]` | text, watermark, human, humanoid | evaluate per case |
| Character with energy features (Saa) | `a humanoid figure of a woman` + energy features described explicitly | text, watermark only | human anchor with lowered `--sw` if bleed occurs |
