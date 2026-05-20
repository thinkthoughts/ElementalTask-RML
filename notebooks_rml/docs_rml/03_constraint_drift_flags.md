# Notebook 03 — Constraint Drift Flags

ElementalTask-RML converts emergence ordering and function-vector geometry into lightweight training-monitoring signals.

## Inputs

- Notebook 01 emergence-order outputs
- Notebook 02 function-vector drift outputs

## Monitoring pipeline

`checkpoint → emergence rank → FV geometry → constraint flags`

## Summary

- Checkpoints analyzed: 6
- Pairwise component → composite constraints: 4

## Monitor flag counts

|                                                            |   0 |
|:-----------------------------------------------------------|----:|
| recovering                                                 |   2 |
| high_fv_drift;fv_geometry_unstable                         |   2 |
| high_fv_drift;fv_geometry_unstable;fv_constraint_violation |   1 |
| stable                                                     |   1 |

## Schedule flag counts

|                 |   0 |
|:----------------|----:|
| behind_schedule |   4 |

## Figures

![Constraint Drift Flags](../figures/03_constraint_drift_flags.png)

![Geometry Recovery](../figures/03_geometry_recovery.png)

![Ahead / Behind Schedule](../figures/03_ahead_behind_schedule.png)

## Interpretation

ElementalTask suggests emergence ordering and function-vector geometry become increasingly stable during training.

This notebook explores whether lightweight monitoring heuristics can detect unstable emergence, capability ordering violations, and geometry drift before training completion.

Emergence ≠ magic. Monitor constraints. 📐
