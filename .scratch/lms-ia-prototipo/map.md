# LMS potenciado por IA — Prototipo

Labels: `wayfinder:map`

## Destination

Dos prototipos navegables (HTML estático + IndexedDB) listos para mostrar a docentes y estudiantes reales: uno que responda "¿el docente siente que gana control y libera tiempo?", otro que responda "¿el estudiante ve que le aporta valor?".

## Notes

- Formato: HTML estático + IndexedDB para persistencia y simulación de respuestas IA
- Audiencia de los prototipos: docentes y estudiantes universitarios (decisores institucionales con background docente también)
- **Este mapa incluye ejecución** — los tickets de construcción son parte del mapa, no solo decisiones
- Skills a consultar: `/prototype`, `/grilling`

### Conceptos clave del sistema

- **Dos carriles paralelos**: camino estándar (diseñado y controlado por el docente, siempre accesible) + carril personalizado (generado por el agente, opt-in del estudiante habilitado por el docente)
- **Agente instructional designer**: ayuda al docente a crear el camino estándar con fundamento pedagógico; reduce el coste de diseño del curso
- **Reporting agregado al docente**: debilidades y fortalezas de la clase sin corrección manual; detalle individual solo bajo demanda explícita
- **Privacidad por diseño**: personalización basada en datos que el estudiante aporta voluntariamente y puede eliminar; RGPD-compatible
- **Evaluación sumativa siempre humana**: el agente hace corrección formativa; la calificación oficial queda fuera de su alcance por exigencia institucional

### Hallazgos de la validación previa (`.scratch/lms-ia-validacion/`)

La validación completada antes de este mapa estableció cuatro conclusiones que enmarcan cada decisión de diseño del prototipo:

**1. El mercado está bifurcado y el hueco existe**
Los LMS institucionales (Canvas, Moodle) han añadido IA de forma superficial — son gestores con chatbot. Los agentes IA educativos (Khanmigo, Duolingo Max, Synthesis) son pedagógicamente sofisticados pero operan sobre contenido cerrado y sirven segmentos K-12 o consumidor. Nadie combina LMS completo + agente tutor sobre material propio del docente + educación superior como segmento nativo. Los cinco gaps que el prototipo debe hacer visibles: contenido del docente como base del agente; LMS + agente + herramienta de autor en un solo sistema; docente como arquitecto pedagógico (no productor de contenido); educación superior como segmento prioritario; bucle bidireccional de feedback docente–agente.

**2. Técnicamente viable, con un límite claro**
La arquitectura multi-agente (agente de diálogo + corrección KG-grounded + planificación curricular + reporting) está validada en producción (ITAS, Arapai, ELEVATE, julio 2026). Coste estimado: ~$1/estudiante/mes con modelos optimizados. El único cuello de botella severo es la corrección automática de respuestas abiertas — los LLMs sobre-rechazan válidas y sobre-validan incorrectas (límite arquitectónico, no de prompting). El prototipo no debe insinuar que la calificación sumativa puede ser automática.

**3. Encaje regulatorio resuelto por diseño**
El carril estándar siempre presente resuelve el conflicto con guías docentes formales (ANECA y equivalentes): el material oficial nunca desaparece. El control en capas (docente habilita el carril personalizado; estudiante decide usarlo) permite adopción gradual sin riesgo institucional. La evaluación formal convive como capa separada, compatible con Bolonia.

**4. Propuesta de valor neta para cada actor**
- **Docente**: elimina corrección masiva de práctica y diagnóstico manual del estado de la clase; conserva autoridad sobre el camino estándar y evaluación sumativa; gana reporting proactivo y tiempo para mentorización real.
- **Estudiante**: mayor impacto en los extremos — el motivado sin techo artificial y el rezagado con red de rescate temprana. El estudiante medio-pasivo usa el sistema como LMS normal. Riesgo principal: una respuesta frustrante del agente acelera el abandono; mitigado con detección proactiva y escalado voluntario al docente.

## Decisions so far

- [¿Qué flujo concreto muestra el prototipo del docente?](.scratch/lms-ia-prototipo/issues/01-flujo-prototipo-docente.md) — Dos momentos: creación con agente instructional designer (input libre + interacción iterativa + edición manual) y dashboard con alertas accionables + sugerencias del agente + acciones del docente siempre visibles.
- [¿Qué flujo concreto muestra el prototipo del estudiante?](.scratch/lms-ia-prototipo/issues/02-flujo-prototipo-estudiante.md) — Camino estándar con callejones personalizados activados por resultado (profundización o refuerzo); aha moment: callejón de refuerzo completo con conversación con el agente; mapa acumulado de exploración personal.

## Not yet specified

- Sesiones de reacción con usuarios reales tras construir los prototipos — qué se mide, cómo se recoge el feedback
- Si la reacción confirma el enfoque, qué prototipo adicional puede necesitarse (¿flujo de onboarding institucional? ¿panel de reporting del docente más detallado?)

## Out of scope

<!-- ninguno de momento -->
