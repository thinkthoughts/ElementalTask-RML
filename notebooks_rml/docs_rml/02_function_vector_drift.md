# Notebook 02 — Function-Vector Drift Monitoring

This notebook adds a lightweight function-vector geometry monitor for ElementalTask-RML.

## Outputs

- `figures/02_function_vector_similarity.png`
- `figures/02_function_vector_drift.png`
- `figures/02_fv_rank_stability.png`
- `figures/02_fv_constraint_score.png`
- `results/02_fv_similarity_final.csv`
- `results/02_fv_drift_scores.csv`
- `results/02_fv_constraint_scores.csv`
- `results/02_fv_constraint_details.csv`
- `results/02_fv_monitor_summary.csv`

## Initial interpretation

Function-vector similarity gives a second monitoring layer beyond accuracy curves.

A stable training trajectory should preserve task geometry: similar atomic tasks cluster, compositional tasks remain close to their component tasks, and pairwise geometry drifts less as checkpoint order increases.

Pipeline:

`checkpoint → function-vector geometry → similarity drift → constraint score`

Emergence ≠ magic. Monitor constraints. 📐
