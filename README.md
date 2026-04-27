# ringest_fase_2

This is Phase 2 of the RINGEST series. Phase 1 dataset is required as input (Zenodo DOI `10.5281/zenodo.19813389`).

Phase 2 is a minimal reproducibility repository for the Kerr audit material used in Paper 2. It contains:

- a paper skeleton in `paper/`;
- generated LaTeX tables in `paper/tables/`;
- generated figures in `paper/figures/`;
- scripts that read the real Phase 2 CSV/JSON inputs and emit tables and figures;
- a lightweight copy of the Phase 1 input/output material in `data/`.

The real audit inputs are read from:

- `../RINGEST/runs_sync/active/kerr_audit_20260424_t66_sigmas/`
- `../RINGEST/runs_sync/active/kerr_audit_gwtc4_pseobnr_t82a_verified/`
- `../RINGEST/runs_sync/active/kerr_population_tail_t9/`
- `../RINGEST/runs_sync/active/kerr_snr_systematics_t10/`

See `REPRODUCIBILITY.md` for the exact generation commands.
