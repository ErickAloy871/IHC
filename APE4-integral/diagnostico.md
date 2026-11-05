# Diagnóstico UX

Diagnóstico de experiencia de usuario y definición del problema para el caso de agendamiento de citas médicas.

## Persona y contexto
- **Persona:** Paciente ambulatorio del centro de salud UTA que necesita reservar una cita rápida y autónomamente desde un celular o computador, y no quiere perder la información ingresada si ocurre un error imprevisto.
- **Contexto:** Plataforma web de agendamiento médico de la universidad con alta demanda de turnos, donde los cupos se actualizan dinámicamente.
- **Restricción:** El sistema debe ser completamente operable mediante teclado (:focus-visible, accesibilidad WCAG) y permitir la corrección ágil de errores sin reiniciar el formulario desde cero.
- **Fallo adicional (incidencia):** Concurrencia de reservas en el mismo turno (simulación de horario 10:30 ocupado simultáneamente por otro usuario al confirmar).

## Tareas
- **T1:** Localizar cómo agendar una cita con Medicina general.
- **T2:** Elegir fecha y hora (10:30), ingresar datos del paciente y corregir errores de validación o conflicto de horario.
- **T3:** Finalizar, confirmar la reserva y registrar el código de cita asignado.

## 5 problemas priorizados
| # | Problema | Heurística de Nielsen | Prioridad |
|---|---|---|---|
| 1 | No se sabe qué horarios están ocupados hasta que se elige | Visibilidad del estado del sistema | Alta |
| 2 | El error de horario borra lo ya escrito o reinicia pasos | Control y libertad del usuario | Alta |
| 3 | No hay confirmación clara con código de cita | Retroalimentación | Alta |
| 4 | Mensajes de error vagos en el formulario solo al enviar | Ayuda a reconocer y corregir errores | Media |
| 5 | No se puede cancelar o cambiar una cita fácilmente en 'Mis citas' | Control y libertad del usuario | Media |

## Touchpoints y momentos de verdad
Ver `recorrido-emocional.csv`. Escala: -2 muy negativa, -1 negativa, 0 neutra, 1 positiva, 2 muy positiva.
- **Momentos de verdad:** tp4 (elegir hora) y tp7 (confirmación). Si alguno de estos dos puntos críticos falla, el usuario experimenta frustración y desconfianza en el sistema.
- En la versión v2 se garantiza que ante el error en el momento de verdad tp4/tp5, el usuario disponga de opciones alternativas inmediatas sin perder sus datos.
