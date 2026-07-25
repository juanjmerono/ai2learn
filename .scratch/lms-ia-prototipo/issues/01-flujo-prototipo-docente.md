# ¿Qué flujo concreto muestra el prototipo del docente?

Type: grilling
Status: resolved

## Question

¿Qué pantallas y acciones debe incluir el prototipo del docente para que, al navegarlo, sienta que gana control sobre su asignatura y libera tiempo? ¿Cuál es el momento clave — el "aha moment" — que tiene que vivir dentro del prototipo?

Decidir: flujo de entrada, pantallas principales, qué hace el agente instructional designer visible, cómo aparece el reporting de la clase, qué acciones puede tomar el docente y cuáles delega en el agente.

## Answer

### Estructura del prototipo: dos momentos en secuencia

**Aha moment 1 — Creación de la asignatura**: "el agente me ahorra horas de diseño pero sigo controlando qué se crea"
**Aha moment 2 — Dashboard en marcha**: "sé exactamente dónde están mis estudiantes sin corregir nada, y el sistema me dice qué hacer"

---

### Momento 1: Creación de la asignatura

**Punto de entrada único** — el docente aporta material (cualquier combinación de):
- Documentos propios (PDF, Word, SCORM, IMS CC)
- Guía docente
- URLs y referencias web abiertas

El agente trabaja sobre ese input y puede complementarlo con fuentes abiertas adicionales.

**Flujo de interacción con el agente instructional designer**:
- Conversación iterativa (no one-shot): el docente refina la propuesta del agente con instrucciones en lenguaje natural ("cambia el tono de este módulo", "añade un ejercicio práctico al final", "fusiona estos dos bloques")
- El resultado es una estructura de módulos con: título, objetivo de aprendizaje, tipo de objeto (lección, ejercicio, examen) y **referencias siempre visibles al material original o fuentes abiertas**
- Edición manual disponible como escape hatch para ajustes finos (reordenar bloques, renombrar, editar texto directamente) — el agente es el camino principal, la edición manual existe para no sentirse atrapado

---

### Momento 2: Dashboard de asignatura activa

**Pantalla principal**:
- Alerta destacada en primer plano — algo accionable de inmediato ("3 estudiantes llevan más de una semana sin avanzar en el módulo 2", "el 40% tiene dificultades con el concepto X")
- Junto a cada alerta: **acción sugerida por el agente** ("añadir material de refuerzo al módulo 2 — puedo generarlo ahora")
- Estado general de la clase debajo de las alertas

**Acciones siempre disponibles para el docente**:
- Revisar detalle de un estudiante concreto
- Añadir o modificar material del camino estándar
- Añadir material exclusivo para caminos personalizados
- Revisar conversaciones elevadas de estudiantes atascados
- Aceptar/rechazar sugerencias del agente

El prototipo puede ampliar alguna de estas acciones para mostrar el flujo completo.
