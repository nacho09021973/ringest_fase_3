# ringest_fase_2

[![Phase 1 DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19813389.svg)](https://doi.org/10.5281/zenodo.19813389)
[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](#reproducibility)

This is Phase 2 of the RINGEST series. Phase 1 dataset is required as input (Zenodo DOI `10.5281/zenodo.19813389`).

Phase 2 is a minimal reproducibility repository for the Kerr-audit material used in Paper 2. It turns verified Phase 2 CSV/JSON audit products into manuscript-ready tables, figures, and a paper skeleton.

![T10 SNR-residual diagnostic](paper/figures/t10_snr_residual_by_cohort.png)

## At a Glance

- Input base from Phase 1: `data/phase1_data/` and `data/phase1_outputs/`
- Real audit inputs read from: `../RINGEST/runs_sync/active/`
- Table builder: `scripts/make_tables.py`
- Figure builder: `scripts/make_figures.py`
- Paper skeleton: `paper/paper_gamma_2.tex`

Generated artifacts:

- `paper/tables/t9_population_tail_stats_table.tex`
- `paper/tables/t10_snr_residual_audit_table.tex`
- `paper/tables/t10_overlap_decomposition_table.tex`
- `paper/tables/source_audit_critical_events_table.tex`
- `paper/figures/t10_snr_residual_by_cohort.pdf`
- `paper/figures/t10_1_overlap_shapley.pdf`
- `paper/figures/source_audit_critical_events.pdf`

## Scope

This repository covers the reproducible audit layer for Paper 2:

- T9.2 population-tail NULL audit inputs and tables
- T10 SNR-residual cohort diagnostic
- T10.1 six-event paired Shapley decomposition
- source-audit comparison for the three critical events

It does not re-run the original exploratory pipelines under `RINGEST/runs_sync/active`; those are treated as fixed read-only inputs here.

## Reproducibility

This repository assumes the real Kerr-audit inputs are available under:

`../RINGEST/runs_sync/active`

From the repository root:

```bash
python3 scripts/make_tables.py
python3 scripts/make_figures.py
```

Outputs are written to:

- `paper/tables/`
- `paper/figures/`

Full details are in [REPRODUCIBILITY.md](REPRODUCIBILITY.md).

## Repository Layout

```text
ringest_fase_2/
├── data/
├── paper/
│   ├── figures/
│   ├── tables/
│   ├── paper_gamma_2.tex
│   └── refs.bib
├── scripts/
├── README.md
└── REPRODUCIBILITY.md
```

## Phase 1 Dependency

Phase 1 remains the canonical literature-based dataset package:

- Repository: `https://github.com/nacho09021973/ringest_fase_1`
- Zenodo DOI: `10.5281/zenodo.19813389`
