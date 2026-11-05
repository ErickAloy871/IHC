# Hallazgos

Llenar solo con lo observado en P01 y P02.

| # | Hallazgo | Evidencia | Heurística | Gravedad | ¿Se corrige en v2? |
|---|---|---|---|---|---|
| H1 | Errores de formulario solo al enviar y con texto genérico | P01 y P02 tuvieron errores en formato de teléfono y nombres; la alerta salía solo al enviar y sin formato sugerido | Ayuda a reconocer y corregir errores | Media | Sí (validación onblur con ejemplos y maxlength 10) |
| H2 | El error de reserva ofrecía reintentar la hora ya tomada y obligaba a repetir pasos | Al elegir 10:30 (simulada ocupada), reintentar repetía el fallo y la otra opción devolvía al inicio perdiendo el flujo | Control y libertad del usuario | Alta | Sí (pantalla de error muestra horas libres directas y salto a revisión) |
| H3 | En Mis citas solo se podía cancelar y no reprogramar | Los usuarios no podían modificar fecha/hora sin cancelar y volver a agendar desde cero | Control y libertad del usuario | Media | Sí (botón Reprogramar que conserva datos y libera la cita al confirmar) |

## Revisión de accesibilidad
- Teclado y foco: Cumplido. Flujo 100% navegable con Tab, Enter y Espacio; indicador visual ámbar claro (:focus-visible) en todos los controles interactivos.
- Mensajes sin depender del color: Cumplido. Avisos con texto descriptivo estructurado y atributos aria-live="polite", role="alert" y role="status", garantizando legibilidad ante daltonismo o con lectores de pantalla.
