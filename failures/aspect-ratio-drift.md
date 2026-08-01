# Failure: Aspect-ratio drift

## Signature

The content is broadly correct, but the output uses the wrong ratio or reaches the requested ratio by removing an important subject or background anchor.

## Why it happens

Aspect ratio is treated as a finishing preference instead of a compositional constraint. The model optimizes the scene first and the canvas second.

## Minimal repair

```text
Output exactly [ratio and dimensions]. Preserve [named anchors] inside the
frame at their existing relative scale. Extend or simplify only [permitted
region]. Do not zoom, recenter, or crop a protected anchor.
```

## Verification

- pixel dimensions match;
- protected anchors remain visible;
- subject scale has not changed unintentionally;
- reserved copy or UI safe area still exists.

## Reusable rule

Lock channel, ratio, and safe areas before applying style.
