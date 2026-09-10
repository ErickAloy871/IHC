# Prueba Práctica 1 - Interacción Humano-Computador (IHC)
**Caso de estudio:** Diseño HCI de un mecanismo para la gestión de citas - GABO'S Readaptación y Movimiento.

## Repositorio
**Enlace:** https://github.com/ErickAloy871/IHC

## Integrantes, usuarios y roles

| Apellidos y Nombres | Usuario GitHub | Rol |
|---|---|---|
| Guevara Mauricio | @Mauri10G | Analista de Requerimientos |
| Carvajal Juan | @juanjose1234456787654 | Tester |
| Chicaiza Eduardo | @Junior-eng-software | Desarrollador Frontend |
| López Erick | @ErickAloy871 | QA |

## Issues y commits por integrante

**Guevara Mauricio (Analista de Requerimientos):** Issues para el análisis del proceso actual y la identificación de usuarios; commits con el mapeo del flujo AS-IS (actores, información necesaria, decisiones), las esperas/transcripciones/errores detectados, y la matriz de usuarios y necesidades (Actividad 1 y 2).

**Carvajal Juan (Tester):** Issues orientados a evaluar alternativas de solución; commits con el análisis descriptivo de los cuatro mecanismos de agendamiento, la matriz de decisión ponderada, la selección justificada del mecanismo híbrido, y la operacionalización de los indicadores de eficiencia por cada operación del sistema (Actividad 3 y 4).

**Chicaiza Eduardo (Desarrollador Frontend):** Issues de diseño de interacción; commits con la construcción de las tres metáforas de interfaz exigidas (calendario de citas, camino de regreso y semáforo de estado), incluyendo su justificación en términos de affordances, mapeo, consistencia y retroalimentación (Actividad 5).

**López Erick (QA):** Issues de construcción y verificación del prototipo; commits con las 9 pantallas del prototipo navegable en Figma, la cobertura de los requisitos de usabilidad (navegación, retroalimentación, prevención de errores, estados de carga/error/recuperación), y el protocolo de validación con usuarios (Actividad 6 y 7).

## Pull Requests y revisión cruzada

- **PR #1 (Proceso actual y usuarios):** Creado por Guevara Mauricio ➔ Revisado y aprobado por Carvajal Juan.
- **PR #2 (Comparación de mecanismos e indicadores):** Creado por Carvajal Juan ➔ Revisado y aprobado por Chicaiza Eduardo.
- **PR #3 (Metáforas de interfaz):** Creado por Chicaiza Eduardo ➔ Revisado y aprobado por López Erick.
- **PR #4 (Prototipo HCI y validación):** Creado por López Erick ➔ Revisado y aprobado por Guevara Mauricio.

## Reflexión grupal

El desarrollo de esta práctica permitió comprender cómo la Interacción Humano-Computador transforma un proceso fragmentado en una solución digital centrada en el usuario. A través del análisis del flujo AS-IS en GABO'S Readaptación y Movimiento, identificamos los puntos de fricción que afectaban a pacientes, fisioterapeutas y personal administrativo. La comparación ponderada de mecanismos de agendamiento y la definición de metáforas de interfaz coherentes permitieron materializar un modelo híbrido que automatiza lo rutinario sin eliminar el criterio humano en las excepciones. El trabajo colaborativo mediante control de versiones en GitHub garantizó coherencia entre los problemas detectados en el análisis y las soluciones representadas en el prototipo final. (97 palabras)

## Justificación de Issues

### Justificación Issue 1 — Análisis del proceso actual (AS-IS)
**Responsable:** Guevara Mauricio (Analista de Requerimientos)
**Descripción:** Subida y justificación del diagrama de flujo AS-IS y la identificación de actores.

**Evidencia visual:** Figura 1 — Diagrama de Flujo AS-IS (swimlane Paciente / Personal administrativo / Fisioterapeuta).

<img width="841" height="365" alt="Diagrama de flujo AS-IS con tres carriles: Paciente, Personal administrativo y Fisioterapeuta" src="https://github.com/user-attachments/assets/d9fb9e08-87b7-4a69-a138-f1bb08212ff1" />

**Justificación del diseño:** El diagrama separa a los tres actores en carriles independientes para hacer visible dónde ocurre cada fricción del proceso actual (espera sin tiempo estimado, doble revisión, transcripción manual). Esta representación permite ubicar con precisión los puntos donde el rediseño digital debía intervenir primero.

### Justificación Issue 2 — Usuarios y necesidades
**Responsable:** Guevara Mauricio (Analista de Requerimientos)
**Descripción:** Documentación de la matriz de usuarios, objetivos, necesidades y dificultades actuales (Actividad 2).

**Justificación del diseño:** Se identificaron cuatro tipos de usuario (paciente, fisioterapeuta, personal administrativo, administrador del centro) porque cada uno interactúa con el sistema de forma distinta y necesita una solución distinta. Esta segmentación es la base sobre la que se construyeron después las metáforas de interfaz y el prototipo, evitando diseñar una única pantalla que intente resolver las necesidades de todos por igual.

### Justificación Issue 3 — Comparación de mecanismos y selección del híbrido
**Responsable:** Carvajal Juan (Tester)
**Descripción:** Documentación de la matriz de decisión ponderada entre las cuatro alternativas de agendamiento (Actividad 3).

**Evidencia visual:** Figura 2a — Análisis descriptivo de cada alternativa por criterio.

<img width="943" height="391" alt="Tabla comparativa de criterios para las cuatro alternativas de agendamiento" src="https://github.com/user-attachments/assets/4c7d321d-532a-4d25-aab0-ed88f4f7a246" />

**Evidencia visual:** Figura 2b — Matriz de decisión ponderada (Agenda digital interna / Solicitud con confirmación / Autoagendamiento / Mecanismo híbrido).

<img width="937" height="444" alt="Matriz de decisión ponderada con puntaje final de cada alternativa" src="https://github.com/user-attachments/assets/f7e3ae41-f9c4-470b-9caa-99da5b12460c" />

**Justificación del diseño:** Cada alternativa se evaluó con los mismos diez criterios (tiempo administrativo, prevención de errores, accesibilidad, factibilidad técnica, etc.), ponderados según los puntos de fricción más críticos detectados en el AS-IS. El mecanismo híbrido obtuvo el puntaje más alto (4.40/5) porque automatiza los casos estándar y conserva el criterio humano en las excepciones, sin excluir a los pacientes con menor manejo digital.

### Justificación Issue 4 — Indicadores de eficiencia
**Responsable:** Carvajal Juan (Tester)
**Descripción:** Operacionalización de la eficiencia para las cinco operaciones del sistema: consultar, registrar, modificar, cancelar y reagendar (Actividad 4).

**Justificación del diseño:** Se definieron indicadores más allá del tiempo (tasa de duplicados evitados, porcentaje de confirmaciones entregadas, trazabilidad conservada) porque un proceso más rápido con más errores no representa una mejora real para el centro. Esta decisión metodológica sostiene después el criterio de éxito usado para evaluar el prototipo.

### Justificación Issue 5 — Metáforas de interfaz
**Responsable:** Chicaiza Eduardo (Desarrollador Frontend)
**Descripción:** Diseño y justificación de las tres metáforas de interfaz exigidas (Actividad 5).

**Evidencia visual:** Figura 3 — Calendario y horarios disponibles.

<img width="680" height="510" alt="Calendario mensual con grilla de horarios disponibles para reagendar una cita" src="https://github.com/user-attachments/assets/ceca8809-1a16-4ca8-874d-2ff4a33fc763" />

**Evidencia visual:** Figura 4 — Flecha de regreso y enlaces "Editar".

<img width="691" height="511" alt="Pantalla con flecha de regreso y pantalla de resumen con enlaces Editar por campo" src="https://github.com/user-attachments/assets/38c51f60-2818-42ae-88a7-a86800cb3ad3" />

**Evidencia visual:** Figura 5 — Insignias de estado (semáforo).

<img width="683" height="507" alt="Listado de citas con insignias de estado en verde, ámbar y rojo" src="https://github.com/user-attachments/assets/b5aea893-59b4-4fbd-8ab9-dfa19792a6b0" />

**Justificación del diseño:**
- *Calendario de citas:* solo expone las franjas realmente libres, eliminando la doble revisión manual detectada en el AS-IS.
- *Camino de regreso:* se descartó un stepper numerado por tratarse de una app móvil; la flecha de retroceso y los enlaces "Editar" permiten corregir un dato puntual sin reiniciar el flujo.
- *Semáforo de estado:* insignias de color con texto (nunca solo color, por accesibilidad) que resuelven la falta de retroalimentación que sufría el paciente en el proceso actual.

### Justificación Issue 6 — Prototipo navegable en Figma
**Responsable:** López Erick (QA)
**Descripción:** Construcción de las 9 pantallas del prototipo y verificación de los 6 requisitos generales de usabilidad (Actividad 6).

**Evidencia visual:** Figura 6 — Inicio.

<img width="251" height="486" alt="Pantalla de inicio con próxima cita, botones Agendar nueva cita y Ver mis citas" src="https://github.com/user-attachments/assets/5a44c965-c7e2-49d6-b9ec-011782561cb8" />

**Evidencia visual:** Figura 7 — Selección de fisioterapeuta.

<img width="247" height="488" alt="Pantalla de selección de fisioterapeuta con tarjetas de cada profesional" src="https://github.com/user-attachments/assets/38377578-331b-4952-b449-29995f41e233" />

**Evidencia visual:** Figura 8 — Datos del paciente (validación inline).

<img width="668" height="495" alt="Formulario de datos del paciente vacío y completo, con validación de campos" src="https://github.com/user-attachments/assets/c5139b27-e083-41ea-9f48-1c11966c0925" />

**Evidencia visual:** Figura 9 — Resumen y confirmación.

<img width="662" height="487" alt="Pantalla de resumen de cita con enlaces Editar y botón Confirmar cita" src="https://github.com/user-attachments/assets/2c32515a-be41-495b-bdb6-86f687bd4a26" />

**Evidencia visual:** Figura 10 — Detalle de cita.

<img width="672" height="491" alt="Pantalla de detalle de cita confirmada con botones Reagendar y Cancelar cita" src="https://github.com/user-attachments/assets/f3a0f393-aeb1-492d-8923-1ae10a6055f3" />

**Evidencia visual:** Figura 11 — Reagendamiento.

<img width="667" height="490" alt="Pantalla de reagendamiento con calendario y grilla de nuevos horarios disponibles" src="https://github.com/user-attachments/assets/271042a4-2c80-45fd-87dc-e58998e87961" />

**Evidencia visual:** Figura 12 — Guardando cita / Error de conexión.

<img width="657" height="486" alt="Pantalla de carga Guardando tu cita y pantalla de error de conexión con botón Reintentar" src="https://github.com/user-attachments/assets/e1fac097-ef5b-4b5f-80a9-62ac1c44d6cb" />

**Evidencia visual:** Figura 13 — Modal de cancelación.

<img width="231" height="485" alt="Modal de confirmación explícita antes de cancelar una cita" src="https://github.com/user-attachments/assets/2168ac8f-d52f-40f0-a140-67169f1a4507" />

**Evidencia visual:** Figura 14 — Mis citas.

<img width="234" height="480" alt="Listado Mis citas con pestañas de filtro y tarjetas con insignia de estado" src="https://github.com/user-attachments/assets/28593717-379b-4adf-8374-c5ac6fe37505" />

**Documentación de diseño y usabilidad:**
- **Reconocimiento antes que recuerdo:** el resumen de cita muestra todos los datos seleccionados de forma explícita antes de confirmar, sin que el paciente deba recordar lo ingresado en pasos previos.
- **Retroalimentación inmediata:** al confirmar, el sistema muestra una pantalla de carga con progreso por pasos y, al finalizar, el detalle de cita con su estado visible.
- **Prevención de errores (heurística de Nielsen):** la cancelación exige una confirmación explícita en un modal, y la grilla de horarios nunca muestra un horario ya ocupado como opción seleccionable.
- **Ruta de recuperación ante errores:** si falla la conexión al guardar, la interfaz muestra un mensaje comprensible, el código técnico del error, y un botón "Reintentar" que conserva los datos ya ingresados.
- **Ley de Proximidad:** en el Detalle de cita, los datos del fisioterapeuta y del paciente se agrupan visualmente por bloques relacionados.

### Justificación Issue 7 — Protocolo de validación
**Responsable:** López Erick (QA)
**Descripción:** Diseño del protocolo de prueba de usabilidad con 3 participantes y 5 tareas (Actividad 7).

**Justificación del diseño:** Se definieron perfiles de participantes deliberadamente distintos (uno con manejo digital fluido, uno con manejo digital limitado, y un miembro del personal administrativo) porque el AS-IS mostró que GABO'S atiende a pacientes con niveles de alfabetización digital muy variados. Medir tiempo, acciones, intervención necesaria y errores por tarea permite validar si el mecanismo híbrido realmente reduce la fricción para todos los perfiles, no solo para el usuario ideal.

## Recomendaciones

- Ejecutar las pruebas de usabilidad reales del protocolo de la Actividad 7 con los 3 perfiles de participantes antes de avanzar a una eventual etapa de desarrollo.
- Conectar el prototipo a un backend real permitiría verificar en producción los indicadores de eficiencia definidos en la Actividad 4 (tasas de duplicados evitados, confirmaciones entregadas, trazabilidad conservada).

## Link prototipo:

[https://www.figma.com/make/WClEJSdhHVASlQs67uVQSY/Mockups-para-app-de-citas?p=f&t=kTjzdPw8XvLdWtE9-0](https://www.figma.com/make/WClEJSdhHVASlQs67uVQSY/Mockups-para-app-de-citas?code-node-id=0-6&p=f&t=KIsHBmPj7LxlQB5v-0&fullscreen=1)
