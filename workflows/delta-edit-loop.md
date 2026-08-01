# Workflow: Delta-edit loop

## Purpose

Change one visible property without paying the risk of an unnecessary full regeneration.

## Procedure

1. Name what already passes.
2. Name the single failed delta.
3. Restate the locks.
4. Specify the affected region.
5. Match local light, texture, perspective, sharpness, and noise.
6. Reject any collateral change.
7. Save the successful repair language.

## Critique template

```text
KEEP
- [what is already correct]

CORRECT ONLY
- [one failed property] in [specific region]

MATCH
- [light, perspective, texture, sharpness, noise, type style]

LOCK
- [identity, camera, geometry, other text, background anchors]

REJECT IF
- [observable collateral change]
```

## Example

```text
Keep the composition, subject, lighting, border, and all other copy.
Correct only the misspelled two-word headline in the top-left block.
Match the existing condensed type weight, baseline, spacing, and ink texture.
Reject the result if any character, object, color, or crop changes.
```

## When not to use it

Use a full regeneration when:

- the core concept is wrong;
- the camera geometry cannot support the goal;
- the desired change affects most of the image;
- the output has several coupled failures;
- the model repeatedly ignores local masks or regions.
