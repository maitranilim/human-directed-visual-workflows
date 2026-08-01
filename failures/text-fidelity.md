# Failure: Text fidelity

## Signature

The poster or UI looks convincing at a glance, but words are misspelled, labels mutate, small copy becomes nonsense, or type changes outside the requested region.

## Why it happens

Image synthesis is asked to perform exact typesetting and visual composition simultaneously.

## Minimal repair

For exploration:

```text
Reserve clear text zones and render only the short exact headline.
Use neutral placeholders for small copy.
```

For production:

1. generate the image and hierarchy;
2. remove or ignore generated fine text;
3. recreate all final copy in a deterministic design tool;
4. proofread names, numbers, claims, and calls to action;
5. test contrast and accessibility.

## Reusable rule

Treat generated typography as concept art unless exact copy has been independently verified.
