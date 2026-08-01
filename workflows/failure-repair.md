# Workflow: Failure repair

## Classify first

| Failure | First repair |
|---|---|
| Wrong ratio or crop | Restate exact canvas and protected anchors before style |
| Camera-angle drift | Lock horizon, angle, perspective, and subject scale |
| Identity drift | Reduce stylization and enumerate identity features |
| Over-editing | Use a named local region and “change only” rule |
| Artificial saturation | Specify color roles, highlight control, and source-matched texture |
| Text corruption | Separate art generation from deterministic typesetting |
| Style soup | Keep one primary and at most two supporting style families |
| Decorative UI | Define the information task and interaction state before visual language |
| Cultural inaccuracy | Stop, verify with a qualified source or reviewer, then regenerate |

## Convert the repair into a reusable asset

After a successful correction:

1. rewrite the repair without task-specific names;
2. name the failure it prevents;
3. list categories where it applies;
4. record a known conflict;
5. test it in one different task;
6. promote it to `prompt-library/` only after repeat success.

## Stop rule

Stop iterating when the output passes the predeclared quality threshold and any remaining improvement would be subjective or better handled in a deterministic design tool.
