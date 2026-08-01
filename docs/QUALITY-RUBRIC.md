# Visual quality rubric

Score each dimension from 0 to 2.

| Dimension | 0 | 1 | 2 |
|---|---|---|---|
| Job fit | Attractive but unrelated | Partially serves the audience | Clearly serves the deliverable and channel |
| Composition | Uncontrolled or drifting | Mostly usable | Deliberate hierarchy and stable camera logic |
| Preservation | Locked elements changed | Minor unintended drift | All declared invariants preserved |
| Locality | One request changed the whole image | Some collateral change | Only the requested delta changed |
| Naturalism | Fake texture, light, or saturation | Mixed realism | Believable within the intended medium |
| Style coherence | Keyword collage | Mostly coherent | Every style choice reinforces one direction |
| Text fidelity | Wrong or unreadable | Needs manual correction | Exact, legible, and hierarchically sound |
| Cultural or brand accuracy | Misleading or careless | Unverified | Reviewed and contextually appropriate |
| Rights and privacy | Unsafe to publish | Unclear status | Source and output are safe for intended use |
| Reusability | No record of what worked | Whole prompt saved | Functional fragments and failure notes saved |

## Acceptance

- **17 to 20:** candidate for a polished public sample
- **13 to 16:** usable experiment with explicit limitations
- **8 to 12:** preserve as failure evidence or revise
- **0 to 7:** do not publish as representative work

These are internal review thresholds, not validated industry standards.

## Text-heavy outputs

Image models can produce convincing hierarchy while rendering unreliable small text. For posters and UI concepts, visual quality does not authorize publication. Exact copy should be recreated or verified in a deterministic design tool.
