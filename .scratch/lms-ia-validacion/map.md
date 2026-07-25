# LMS potenciado por IA — Validación de la idea

Labels: `wayfinder:map`

## Destination

Determinar si un LMS agéntico para educación superior es una idea diferenciada, técnicamente viable y con un rol docente claro — con suficiente evidencia para decidir si merece la pena pasar a la siguiente fase (prototipo).

## Notes

- Dominio: EdTech / educación superior (universidad, formación profesional de grado superior)
- El estudiante dispone de un agente tutor que personaliza su itinerario partiendo de un material base creado por el docente
- El agente puede generar ejercicios personalizados, adaptar contenido, mantener el engagement y reportar debilidades al docente
- El docente crea el material base (la "red de seguridad" para estudiantes no interactivos), revisa el estado de la clase y toma decisiones sobre el material
- Las funciones LMS tradicionales (motor de exámenes, calificación, comunicación) siguen siendo necesarias
- La herramienta de autor clásica podría quedar obsoleta si la IA construye el contenido dinámicamente
- Skills a consultar por sesión: `/grilling`, `/domain-modeling`, `/research`

## Decisions so far

- [¿Qué herramientas similares existen ya en el mercado?](.scratch/lms-ia-validacion/issues/01-mercado-herramientas-similares.md) — El mercado está bifurcado: LMS institucionales (Canvas, Moodle) con IA superficial vs. agentes IA educativos (Khanmigo, Duolingo Max) sobre contenido cerrado y segmento K-12; ningún producto combina LMS completo + agente tutor sobre material propio del docente + educación superior como segmento nativo.
- [¿Es técnicamente viable un agente tutor con las herramientas actuales?](.scratch/lms-ia-validacion/issues/03-viabilidad-tecnica-agente-tutor.md) — Sí, viable con arquitectura multi-agente (diálogo + corrección KG-grounded + planificación curricular + reporting); la corrección automática sumativa es el cuello de botella más severo; costes ~$1/estudiante/mes con modelos optimizados.
- [¿Encaja el modelo agéntico en el contexto de educación superior?](.scratch/lms-ia-validacion/issues/02-encaje-educacion-superior.md) — Encaja bien: dos carriles paralelos (estándar + personalizado), control en capas docente/estudiante, ganchos de adopción vía reporting y agente instructional designer; la evaluación formal queda como capa separada compatible con Bolonia.
- [¿Qué valor único aporta el docente en este ecosistema?](.scratch/lms-ia-validacion/issues/04-valor-del-docente.md) — El docente es experto en la materia, supervisor del camino estándar y mentor escalable; el agente absorbe diagnóstico, práctica y diseño pedagógico; la evaluación sumativa sigue siendo humana por exigencia institucional.
- [¿Qué valor percibe el estudiante y qué fricciones puede encontrar?](.scratch/lms-ia-validacion/issues/05-perspectiva-estudiante.md) — Mayor impacto en extremos (motivado y en riesgo); privacidad por diseño (datos bajo control del estudiante, reporting agregado al docente); transparencia total sobre la IA; escalado voluntario al docente como red de seguridad.

## Not yet specified

- Si la validación confirma la idea, qué forma debería tener un primer prototipo (quién lo usa, qué flujo muestra)
- Cómo se mide el éxito del agente tutor (métricas de aprendizaje, engagement, notas)
- Modelo de negocio / go-to-market (SaaS institucional, freemium, licencia, etc.)

## Out of scope

<!-- ninguno de momento -->
