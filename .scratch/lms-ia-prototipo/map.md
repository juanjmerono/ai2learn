# LMS potenciado por IA — Prototipo

Labels: `wayfinder:map`

## Destination

Dos prototipos navegables (HTML estático + IndexedDB) listos para mostrar a docentes y estudiantes reales: uno que responda "¿el docente siente que gana control y libera tiempo?", otro que responda "¿el estudiante ve que le aporta valor?".

## Notes

- Contexto: este esfuerzo parte de la validación completada en `.scratch/lms-ia-validacion/`
- Formato: HTML estático + IndexedDB para persistencia y simulación de respuestas IA
- Audiencia de los prototipos: docentes y estudiantes universitarios (decisores institucionales con background docente también)
- **Este mapa incluye ejecución** — los tickets de construcción son parte del mapa, no solo decisiones
- Skills a consultar: `/prototype`, `/grilling`
- Conceptos clave del sistema:
  - Dos carriles paralelos: camino estándar (docente) + carril personalizado (agente, opt-in estudiante)
  - Agente instructional designer para el docente
  - Reporting agregado al docente, detalle individual bajo demanda
  - Privacidad por diseño: datos del estudiante bajo su control
  - Evaluación sumativa siempre humana

## Decisions so far

- [¿Qué flujo concreto muestra el prototipo del docente?](.scratch/lms-ia-prototipo/issues/01-flujo-prototipo-docente.md) — Dos momentos: creación con agente instructional designer (input libre + interacción iterativa + edición manual) y dashboard con alertas accionables + sugerencias del agente + acciones del docente siempre visibles.
- [¿Qué flujo concreto muestra el prototipo del estudiante?](.scratch/lms-ia-prototipo/issues/02-flujo-prototipo-estudiante.md) — Camino estándar con callejones personalizados activados por resultado (profundización o refuerzo); aha moment: callejón de refuerzo completo con conversación con el agente; mapa acumulado de exploración personal.

## Not yet specified

- Sesiones de reacción con usuarios reales tras construir los prototipos — qué se mide, cómo se recoge el feedback
- Si la reacción confirma el enfoque, qué prototipo adicional puede necesitarse (¿flujo de onboarding institucional? ¿panel de reporting del docente más detallado?)

## Out of scope

<!-- ninguno de momento -->
