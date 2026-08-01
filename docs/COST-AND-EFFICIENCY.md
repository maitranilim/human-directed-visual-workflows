# Cost and efficiency

## Supported qualitative finding

Across repeated use, `maitranilim` reports:

- fewer regenerations;
- faster completion;
- reuse of successful prompt fragments.

The mechanism is plausible and inspectable: preservation locks reduce accidental drift, modular fragments reduce prompt rewriting, and delta critiques reduce full-image restarts.

## What is not yet supported

The historical experiments did not consistently record:

- number of generations;
- elapsed minutes;
- model or pricing tier;
- token or image cost;
- acceptance score;
- baseline workflow;
- downstream design-edit time.

Therefore this repository does not claim a percentage reduction, a monetary saving, or a universal productivity gain.

## Cost-reduction levers

| Lever | Cost it targets | Rule |
|---|---|---|
| Preservation locks | Regenerations caused by unwanted drift | State invariants separately and test them |
| Modular fragments | Prompt rewriting | Reuse only the functional fragment needed |
| Delta critique | Full-composition restarts | Name one failed difference at a time |
| Negative constraints | Repeated known failures | Turn each failure into a reusable guardrail |
| Early channel lock | Wrong dimensions or crop | Set aspect ratio before style exploration |
| Text separation | Failed text rendering | Generate art and set exact copy deterministically |
| Stop rule | Endless subjective iteration | Define acceptance threshold before generation |

## Prospective claim rule

After at least 10 comparable tasks per workflow:

1. compute median generations to acceptance;
2. compute median elapsed minutes;
3. compare new and baseline workflows;
4. preserve the same task class and quality bar;
5. report sample size and variance;
6. publish negative or null results too.
