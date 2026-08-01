# Failure catalog

Failures are preserved because they are the raw material of a reusable workflow.

| Failure | Signature | Minimal first repair |
|---|---|---|
| [Aspect-ratio drift](aspect-ratio-drift.md) | Correct idea, wrong canvas or destructive crop | Lock ratio, dimensions, and protected anchors first |
| [Camera or identity drift](camera-and-identity-drift.md) | New angle, changed proportions, face no longer stable | Enumerate camera and identity invariants |
| [Non-local editing](non-local-editing.md) | One requested change alters unrelated regions | Name the region and reject all collateral change |
| [Artificial naturalism](artificial-naturalism.md) | Plastic texture, fake saturation, dramatic relight | Match source light, noise, sharpness, and restraint |
| [Text fidelity failure](text-fidelity.md) | Layout looks plausible but copy is wrong | Separate concept art from deterministic typesetting |
| [Style-stack overload](style-stack-overload.md) | Many keywords, no coherent visual decision | One primary style and functional supports only |

## Failure record template

```text
Goal:
Locked properties:
Observed failure:
Likely cause:
Smallest repair:
Verification check:
Reusable negative constraint:
Evidence:
Open limitation:
```

Historical failures are reconstructed from available interaction evidence. Where the original failed image is private or unavailable, the repository preserves the behavior signature and repair rather than pretending to show a before-and-after test.
