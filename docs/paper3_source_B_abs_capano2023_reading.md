# Paper 3 — Source B_abs candidate: Capano et al. 2023

## Rol

Candidato principal actual para fuente `B_abs` focal en Paper 3.

Evento esperado:

- GW190521

## Fuente primaria pendiente

Capano et al., "Multimode Quasinormal Spectrum from a Perturbed Black Hole", Phys. Rev. Lett. 131, 221402 (2023), arXiv:2105.05238.

## Estado

No se ha creado YAML B.

No se ha transcrito ningún valor QNM.

Este documento existe para registrar la lectura primaria antes de decidir si la fuente entra como `B_abs`.

## Preguntas de lectura

La fuente primaria debe responder:

1. ¿Reporta valores absolutos de frecuencia en Hz?
2. ¿Reporta tiempos de damping en ms?
3. ¿Qué evento(s) analiza explícitamente?
4. ¿Qué modo(s) identifica o asocia: 220, 221, 330 u otros?
5. ¿Las incertidumbres son simétricas, intervalos creíbles asimétricos o solo posterior plots?
6. ¿Las cantidades están en detector frame, source frame o no queda claro?
7. ¿El método es agnóstico/frequency-domain o impone relaciones Kerr?
8. ¿La tabla/texto permite construir una fila comparable con baseline A para GW190521?
9. ¿Hay material suplementario o data release que deba usarse antes que el texto principal?
10. ¿Los dos picos reportados, si existen, corresponden a modos físicos identificables o a resonancias agnósticas etiquetadas a posteriori?

## Criterio de aceptación como B_abs

Capano et al. 2023 entra como `B_abs` inicial solo si se puede documentar con fuente primaria:

- `event_id = GW190521`
- `source_paper`
- `mode` o etiqueta de resonancia agnóstica claramente mapeable
- `f_hz`
- incertidumbre de frecuencia o intervalo creíble
- `tau_ms`
- incertidumbre de tau o intervalo creíble
- convención de marco
- notas sobre identificación modal

## Decisión pendiente

Tras leer la fuente primaria, decidir:

- `accept_B_abs`: crear YAML mínimo para Capano/GW190521.
- `accept_B_abs_agnostic_labels`: crear YAML con etiquetas agnósticas si no hay modo Kerr inequívoco.
- `needs_more_provenance`: falta tabla/data release o convención.
- `reject_tabular`: no sirve como fuente tabular comparable.
