# Workflow: Reference-preserving edit

## 1. Inventory the reference

Record:

- aspect ratio;
- camera angle;
- horizon and perspective;
- subject position and scale;
- identity-sensitive features;
- dominant color relationships;
- light direction and softness;
- texture, sharpness, and noise;
- background anchors;
- exact text.

## 2. Separate lock from change

Do not combine both in one vague sentence.

```text
LOCK: [explicit invariant list]
CHANGE: [one target and region]
```

## 3. Define source fidelity

Choose:

- strict preservation;
- recognizable preservation with controlled stylization;
- composition reference only;
- mood reference only.

Never let the model infer the fidelity level from “inspired by.”

## 4. Generate

Use the smallest transformation that can satisfy the brief. If the tool supports a local edit or mask, prefer it for local changes.

## 5. Compare

Check in this order:

1. identity and rights;
2. camera and geometry;
3. semantic content;
4. requested delta;
5. lighting and material match;
6. aesthetic polish.

Polish cannot compensate for a broken lock.

## 6. Archive

Record the lock set, tool, accepted iteration, and any failure-specific negative constraint. Do not archive a private source in the public repository.
