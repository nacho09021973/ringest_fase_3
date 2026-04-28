# Paper 3 — Literature triage notes

## Fuente de esta nota

Esta nota resume el informe local:

`docs/Auditar Heterogeneidad QNM Ringdown Gravitacional.pdf`

El PDF se usa como triage bibliográfico interno, no como fuente primaria de valores QNM.

## Estado

Este documento registra el triage bibliográfico recibido para seleccionar fuentes B/C/D/E.

No autoriza todavía la creación de YAML B ni la transcripción de valores numéricos.

## Clasificación operativa

| Clase | Significado |
|---|---|
| B_abs | Fuente con valores absolutos comparables: `f_hz`, `tau_ms` o equivalentes convertibles con provenance directa |
| B_param | Fuente con desviaciones fraccionales respecto a Kerr: `delta_f`, `delta_tau`, `delta_omega_R`, `delta_omega_I`, etc. |
| No_tabular | Fuente metodológica o contextual sin tabla observacional directamente comparable |

## Candidatos identificados por el triage

| Candidato | Evento(s) | Clasificación provisional | Uso inicial |
|---|---|---|---|
| LVK/TGR GWTC-2/3 | 19 eventos baseline A | B_param | No empezar aquí; requiere decisión de transformación |
| Isi et al. 2019 | GW150914 | B_abs provisional | Primer candidato absoluto |
| Capano et al. 2023 | GW190521 | B_abs provisional | Segundo candidato absoluto |
| Giesler et al. 2019 | NR / GW150914-like | No_tabular | Discusión sobre sobretonos y tiempo de inicio |
| Finch & Moore 2022 | GW150914 | No_tabular provisional | Discusión de estabilidad/sensibilidad |

## Decisión práctica

Para probar Fase 3, empezar por fuentes absolutas focales:

1. Isi et al. 2019 para GW150914.
2. Capano et al. 2023 para GW190521.

No empezar por `B_param` LVK/TGR hasta decidir formalmente si la matriz A/B/C/D/E comparará desviaciones parametrizadas además de observables absolutos.

## Reglas de cautela

- No usar el PDF de triage como fuente primaria de valores.
- No transcribir números desde fuentes secundarias.
- Verificar cada valor contra paper oficial, arXiv o data release.
- Si una fuente reporta intervalos creíbles asimétricos, no convertirlos a sigma simétrica sin documentar la regla.
- Si una fuente reporta desviaciones parametrizadas, no forzarla al esquema `f_hz/tau_ms`.
- El PDF sirve para priorizar lectura, no para poblar YAML.

## Próxima acción

Leer la fuente primaria de Isi et al. 2019 para GW150914 y decidir si permite crear un YAML `B_abs` mínimo.
