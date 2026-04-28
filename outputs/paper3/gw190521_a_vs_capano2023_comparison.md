# GW190521 — baseline A vs Capano 2023 (preliminary reporting comparison)

Esta es una comparación preliminar de **reporting**, no un test físico.

## Selección

- Baseline A: `event_id=GW190521`, `mode=220` desde `outputs/paper3/baseline_a_coverage.csv`.
- Capano 2023: resonancia con `kerr_identification=220_candidate` desde `data/phase1_data/qnm_events_capano2023.yml`.
- Fuente B: `Capano et al., Phys. Rev. Lett. 131, 221402 (2023)`.

## Valores comparados

| Magnitud | Baseline A (220) | Capano 2023 (range A / 220_candidate) |
|---|---|---|
| f_hz | 68.0 ± 4.0 | 63.0 +2.0/-2.0 |
| tau_ms | 15.8 ± 3.2 | 26.0 +8.0/-6.0 |

## Intervalos derivados

| Magnitud | A_low | A_high | B_low | B_high |
|---|---:|---:|---:|---:|
| f_hz | 64.0 | 72.0 | 61.0 | 65.0 |
| tau_ms | 12.6 | 19.0 | 20.0 | 34.0 |

## Diferencias brutas (sin estadística)

- delta_f_hz = f_B - f_A = -5.0
- delta_tau_ms = tau_B - tau_A = 10.2

## Solapamiento de intervalos

- f intervals overlap: **True**
- tau intervals overlap: **False**

## Cautelas

- No se calculan p-values ni residual sigma combinado.
- Los intervalos de Capano son asimétricos y se preservan así; no se han simetrizado.
- La Capano range B / 330_candidate queda fuera de esta comparación porque baseline A no contiene 330 para GW190521.
- Esto es un estudio de caso de reporting heterogeneity, no una afirmación de tensión física.
