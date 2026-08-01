# Composition controls

## Control vocabulary

| Control | Values or examples | Why it matters |
|---|---|---|
| Canvas | 1:1, 4:5, 16:9, 9:16, exact pixels | Prevents late destructive crops |
| Camera | Eye level, low angle, overhead, macro, telephoto compression | Stabilizes spatial logic |
| Subject anchor | Center, upper third, lower-left, edge crop | Makes placement inspectable |
| Scale | Face-first, waist-up, full body, environmental | Controls narrative distance |
| Negative space | Top headline, left copy block, safe mobile region | Reserves function before decoration |
| Hierarchy | Primary subject, secondary cue, tertiary annotation | Prevents equal-weight clutter |
| Border system | Open canvas, editorial frame, scanner frame, bleed | Defines the visual container |
| Direction | Symmetric, asymmetric, diagonal, circular, nested | Controls movement |

## Prompt block

```text
COMPOSITION
- Output: [ratio and dimensions].
- Camera: [angle and lens feel].
- Primary subject: [anchor and scale].
- Preserve: [important background anchors].
- Reserve: [negative-space region] for [copy or UI].
- Reading order: [first] -> [second] -> [third].
- Keep all critical content inside [safe-area rule].
```

## Reference-preserving crop example

```text
Create a 4:5 crop without inventing a new camera position. Keep the dominant
cloud mass as the primary background anchor and preserve the smaller celestial
element on the right. Remove only the distracting wire. Do not enlarge,
recenter, or replace either anchor.
```

## Local edit box

For a one-element edit, describe the affected region:

```text
Edit only the upper-right caption zone. Preserve the subject, background,
lighting, border, and all other text exactly.
```
