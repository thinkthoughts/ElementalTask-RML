# Notebook 01 — Emergence Order Monitoring

Source: `synthetic_demo`

Emergence threshold: `0.5`

## Summary

- Tasks analyzed: `6`
- Checkpoints analyzed: `7`
- Pairwise atomic-to-compositional constraints: `6`
- Ordering violations: `0`
- Minimal CGCS: `1.000000`

## Pipeline

`checkpoint -> emergence rank -> function-vector similarity -> constraint-score drift`

## Generated artifacts

- `results_rml/01_emergence_order_table.csv`
- `results_rml/01_pairwise_constraints.csv`
- `results_rml/01_constraint_scores.csv`
- `results_rml/01_rank_stability_by_checkpoint.csv`
- `plots_rml/01_emergence_order_monitor.png`
- `plots_rml/01_rank_stability_monitor.png`
- `plots_rml/01_cgcs_by_checkpoint.png`

## Interpretation

This notebook tests whether checkpoint-level emergence ordering can serve as a lightweight training monitor.

A useful next step is replacing pairwise string-heuristic constraints with an explicit task graph derived from ElementalTask task metadata.

**Emergence ≠ magic. Monitor constraints. 📐**
