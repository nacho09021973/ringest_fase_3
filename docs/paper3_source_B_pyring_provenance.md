# Paper 3 — Source B pyRing provenance

## Rol

Fuente B candidata para auditar reporting heterogeneity frente al baseline A LVK/TGR GWTC-2.

## Fuente candidata principal

Fuente B candidata: pyRing-related Carullo literature. La fuente tabular exacta queda pendiente de identificación.

Referencias relevantes, separadas para evitar confusión bibliográfica:

- Carullo et al., *Phys. Rev. D* **98**, 104020 (2018) — *Empirical tests of the black hole no-hair conjecture using gravitational-wave observations*; referencia del test de no-hair / parametrized ringdown.
- G. Carullo, *Phys. Rev. D* **103**, 124043 (2021) — *parametrized ringdown spin expansion coefficients formalism*; trabajo distinto al anterior.

Aún no está confirmado que ninguna de las dos referencias contenga una tabla directamente convertible a `f_hz` / `tau_ms` por evento y modo. Eso es exactamente lo que debe resolverse antes de crear el YAML de fuente B.

## Estado

No se ha creado todavía `data/phase1_data/qnm_events_pyring.yml`.

No se ha transcrito ningún valor QNM.

El solape real A/B permanece desconocido hasta extraer una lista explícita de `event_id` desde la fuente B.

## Justificación metodológica

pyRing es metodológicamente distinto del baseline A: análisis bayesiano de ringdown post-merger, con likelihood temporal, modelos de ringdown y tests parametrizados de GR sobre frecuencias y damping times.

## Preguntas que deben resolverse antes de crear el YAML

1. ¿La fuente reporta valores absolutos de `f` y `tau`, o solo desviaciones fraccionales respecto a Kerr?
2. ¿Las incertidumbres son simétricas o intervalos creíbles asimétricos?
3. ¿Las cantidades están en marco detector, marco fuente o unidades geométricas?
4. ¿El damping se reporta como `tau`, `gamma`, `omega_I` o `Q`?
5. ¿Qué eventos del baseline A aparecen realmente?
6. ¿Qué modo se reporta: 220, overtone 221, modos superiores u otro parametrizado?
7. ¿La tabla permite una fila comparable `event_id + mode + f_hz + tau_ms`?
8. ¿Hace falta transformar desviaciones fraccionales usando Kerr(M_final, chi_final)?

## Criterio para aceptar pyRing como fuente B

pyRing entra como fuente B principal solo si puede producirse una tabla trazable con:

- `event_id`
- `source_paper`
- `mode`
- `f_hz` o una transformación explícita hacia `f_hz`
- `sigma_f_hz` o intervalo convertible
- `tau_ms` o una transformación explícita hacia `tau_ms`
- `sigma_tau_ms` o intervalo convertible
- notas claras de convención

## Decisión pendiente

Leer la fuente exacta y decidir si pyRing proporciona observables absolutos directamente comparables con baseline A o si solo permite una comparación en espacio de desviaciones parametrizadas.
