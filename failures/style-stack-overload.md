# Failure: Style-stack overload

## Signature

The prompt contains many fashionable terms, but the result has weak hierarchy, inconsistent materials, and no clear design logic.

## Why it happens

Style names are added as decoration rather than assigned a function.

## Minimal repair

```text
Primary design system: [one style].
Supporting influence: [one style] for [one function].
Optional texture: [one finish].
Remove all other style labels.
```

## Verification

For every style word, point to the visible decision it controls. Delete it if no decision changes.

## Reusable rule

One coherent direction with explicit functions is more controllable than a long style stack.
