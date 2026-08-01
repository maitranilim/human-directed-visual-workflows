# Failure: Non-local editing

## Signature

A request to change one caption, object, color, or region causes unrelated changes to the full image.

## Why it happens

The instruction describes the desired result but does not define an edit boundary or reject collateral change.

## Minimal repair

```text
Edit only [target] inside [region]. Keep the full canvas, subject, background,
light, palette, geometry, and every other text element unchanged. Reject any
result with a change outside the named region.
```

## Verification

Use a blink comparison or image-difference view when possible. Check locked regions before assessing the new target.

## Reusable rule

For one-element changes, specify both the local target and the unchanged global state.
