# Preservation locks

Preservation locks define what a generation or edit is not allowed to change.

## Lock classes

| Class | Examples |
|---|---|
| Identity | Face structure, skin tone, age, expression, distinctive marks |
| Camera | Angle, focal-length feel, horizon, perspective, crop logic |
| Geometry | Subject proportions, object positions, silhouette, panel count |
| Semantic | Required object, gesture, relationship, event, exact text |
| Style continuity | Lighting direction, material logic, color relationship |
| Brand | Logo geometry, type treatment, brand colors, clear space |
| Template | Recognized composition, character positions, reaction, caption zones |

## Copyable block

```text
PRESERVATION LOCKS
- Keep [identity or subject] unchanged.
- Keep the original camera angle, perspective, crop logic, and relative scale.
- Keep [named anchors] in their original positions.
- Preserve the lighting direction and the relationship between [colors].
- Preserve exact text: “[text]”.

ALLOWED DELTA
- Change only [target].

DO NOT
- Recompose the scene.
- beautify or stylize locked features;
- add, remove, or replace unrequested objects;
- change aspect ratio;
- rewrite any other text.
```

## Make “same” testable

Weak:

> Keep everything the same.

Stronger:

> Preserve the face shape, expression, skin tone, camera angle, shoulder position, background geometry, and 4:5 crop. Change only the jacket color.

## Conflict rule

When a requested change conflicts with a lock, stop and resolve the conflict before generating. Do not silently sacrifice identity, composition, or exact text to satisfy style.

## Public-evidence note

Personal portrait examples are deliberately not published in this repository. The lock system is preserved because the method is reusable even when the source must remain private.
