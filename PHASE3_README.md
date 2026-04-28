# RINGEST — Fase 3 / Paper 3

Esta carpeta contiene el trabajo específico del Paper 3: reporting heterogeneity en observables QNM publicados.

## Estado

Fase 3 nace como copia limpia de fase 2, pero queda separada operacionalmente.

El objetivo no es modificar el pipeline principal ni reabrir extracción propia desde strain crudo. El objetivo es auditar la heterogeneidad entre fuentes publicadas de QNM y medir su impacto sobre conclusiones de consistencia Kerr.

## Documento inicial

- docs/paper3_reporting_heterogeneity_matrix.md

## Input canónico actual

- data/phase1_data/qnm_events_literature.yml

Este input contiene baseline A, basado en LVK/TGR GWTC-2, con 19 eventos.

## Limitación actual

El input actual no contiene todavía fuentes independientes B/C/D/E. Por tanto, permite diagnóstico de cobertura y baseline A, pero no análisis completo de reporting heterogeneity.

## Regla operativa

No tocar ~/ringest_fase_1.
No empujar cambios de fase 3 hacia fase 2.
No reintroducir la antigua rama ESPRIT.
No correr GPU salvo que una pregunta física concreta lo exija.
