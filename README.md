# RINGEST Fase 3 — Paper 3: reporting heterogeneity in QNM observables

## Estado

Workspace de Fase 3 para Paper 3.

Este repositorio queda congelado como base documental y reproducible del análisis de heterogeneidad de reporting en observables QNM/ringdown.

## Pregunta

¿Hasta qué punto diferencias aparentes entre observables QNM publicados pueden explicarse por heterogeneidad de reporting antes de interpretarse como tensión física?

## Resultado principal

Fase 3 documenta dos casos trazables donde `f_hz` solapa entre fuentes, pero `tau_ms` no solapa:

| Evento | Comparación | f_hz | tau_ms |
|---|---|---|---|
| GW190521 | baseline A vs Capano 2023 | solapa | no solapa |
| GW190910_112807 | baseline A vs GWTC-4.0 Table 3 | solapa | no solapa |

## Interpretación permitida

- `tau_ms` parece más frágil que `f_hz` frente a diferencias de reporting en los casos auditados.
- Una discrepancia aislada en `tau_ms` puede ser reporting heterogeneity.
- El resultado justifica separar heterogeneidad documental/metodológica de tensión física.
- Paper 4 debe partir de esta cautela si busca candidatos discovery.

## Qué no afirma este repositorio

Este repositorio no afirma:

- discovery física;
- tensión Kerr;
- evidencia de nueva física;
- conclusión poblacional;
- significancia estadística global;
- que `tau_ms` sea siempre menos fiable que `f_hz`;
- que los dos casos basten para una afirmación universal.

## Artefactos principales

Documentos:

- `docs/paper3_reporting_heterogeneity_matrix.md`
- `docs/paper3_milestone_02_two_case_reporting_heterogeneity.md`
- `docs/paper3_outline.md`

Comparadores ligeros, si existen:

- `outputs/paper3/gw190521_a_vs_capano2023_comparison.csv`
- `outputs/paper3/gw190910_a_vs_gwtc4_table3_comparison.csv`
- `outputs/paper3/baseline_a_coverage.csv`

Fuentes de entrada, si existen:

- `data/phase1_data/qnm_events_capano2023.yml`
- `data/phase1_data/qnm_events_gwtc4_remnants_table3.yml`

## Relación con Fase 4

Fase 4 debe empezar como filtro de discovery condicionado por Fase 3.

La pregunta natural de Fase 4 es:

> Después de controlar heterogeneidad de reporting, evolución de pipeline, parametrización, incertidumbre Kerr y selección de fuente, ¿queda algún patrón físico robusto?

## Reglas de conservación

Este workspace queda congelado como Fase 3.

No debe usarse para:

- recalcular Paper 4;
- añadir candidatos discovery;
- reintroducir ESPRIT;
- modificar outputs históricos;
- inflar conclusiones con N pequeño.

## Reproducibilidad

El repositorio conserva documentación, comparadores ligeros y provenance textual suficiente para reconstruir la narrativa de Paper 3.

Los outputs pesados, si los hubiera, no forman parte del contrato principal de este README salvo que estén explícitamente versionados.
