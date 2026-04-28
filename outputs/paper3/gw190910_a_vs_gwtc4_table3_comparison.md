# GW190910_112807 — baseline A vs GWTC-4.0 Table 3

Esta es una comparación preliminar de **reporting**, no un test físico.

La fuente A_double_prime procede de LVK/GWTC-4.0 Remnants; no es una fuente B externa independiente.

## Selección

- Baseline A: `event_id=GW190910_112807`, `mode=220` desde `outputs/paper3/baseline_a_coverage.csv`.
- A_double_prime: `event_id=GW190910_112807`, `pipeline=pSEOBNRV5PHM`, `table=Table 3` desde `data/phase1_data/qnm_events_gwtc4_remnants_table3.yml`.
- Fuente: `LVK, GWTC-4.0: Tests of General Relativity. III. Tests of the Remnants`.

## Valores comparados

| Magnitud | Baseline A (220) | GWTC-4 Table 3 / pSEOBNRV5PHM (220) |
|---|---|---|
| f_hz | 177.0 ± 8.0 | 174.5 +12.2/-8.4 |
| tau_ms | 5.9 ± 0.65 | 9.49 +3.46/-2.82 |

## Intervalos derivados

| Magnitud | A_low | A_high | A_double_prime_low | A_double_prime_high |
|---|---:|---:|---:|---:|
| f_hz | 169.0 | 185.0 | 166.1 | 186.7 |
| tau_ms | 5.25 | 6.55 | 6.67 | 12.95 |

## Diferencias brutas (sin estadística)

- delta_f_hz = f_A_double_prime - f_A = -2.5
- delta_tau_ms = tau_A_double_prime - tau_A = 3.59

## Solapamiento de intervalos

- f intervals overlap: **True**
- tau intervals overlap: **False**

## Cautelas

- No se calculan p-values ni residual sigma combinado.
- Los intervalos de GWTC-4 Table 3 son asimétricos y se preservan así; no se han simetrizado.
- Los valores IMR-GR internos de Table 3 se preservan en el YAML, pero no sustituyen baseline A.
- Esto es un estudio de caso de reporting heterogeneity, no una afirmación de tensión física con Kerr.
