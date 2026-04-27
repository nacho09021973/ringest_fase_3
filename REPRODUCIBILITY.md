# Reproducibility

This repository assumes the real Kerr-audit inputs are available under:

`../RINGEST/runs_sync/active`

From the repository root, generate manuscript tables and figures with:

```bash
python3 scripts/make_tables.py
python3 scripts/make_figures.py
```

Default outputs:

- `paper/tables/*.tex`
- `paper/tables/table_manifest.json`
- `paper/figures/*.png`
- `paper/figures/*.pdf`
- `paper/figures/figure_manifest.json`

Phase 1 lightweight inputs are copied in:

- `data/phase1_data`
- `data/phase1_outputs`
