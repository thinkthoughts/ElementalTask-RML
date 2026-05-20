# Notebook 04 — Compositional Forecasting

This notebook explored whether component-task emergence and function-vector geometry can forecast compositional capability emergence.

## Inputs

- emergence order table from Notebook 01
- function-vector similarity/drift outputs from Notebook 02
- optional monitoring flags from Notebook 03

## Forecast heuristic

`predicted checkpoint = max(component checkpoints) + geometry penalty + instability penalty + spread penalty`

## Metrics

|   n_composites |   mae |    rmse |   mean_signed_error |   normalized_mae |
|---------------:|------:|--------:|--------------------:|-----------------:|
|              2 | 79500 | 79916.7 |              -79500 |            0.795 |

## Interpretation

Component emergence and function-vector geometry provide a lightweight, interpretable way to estimate compositional emergence.

This does not claim a general predictive law. It provides a monitoring heuristic that can be compared against real checkpoint trajectories.

Emergence ≠ magic. Monitor constraints. 📐
