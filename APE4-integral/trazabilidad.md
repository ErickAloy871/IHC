# Matriz de trazabilidad

| Req. | Necesidad de usuario | Flujo o decisión | Pantalla o componente | Caso de prueba | Hallazgo y cambio |
|---|---|---|---|---|---|
| R1 | Acceder a la operación | Inicio, Agendar | Inicio, botón principal | T1 | Sin cambio |
| R2 | Elegir especialista y hora | Especialidad, Horario | Lista de médicos, botones de hora | T1 | Sin cambio |
| R3 | Saber qué hora está libre | Horario, hora ocupada | Botones deshabilitados | T1 | Sin cambio |
| R4 | Ingresar y modificar datos | Datos, validación | Campos, mensajes de error | T2 | H1, validación en línea onblur |
| R5 | Corregir el error | Confirmar, error, otra hora | Pantalla de error | T2-E | H2, recuperación en un clic |
| R6 | Finalizar con confirmación | Confirmar, éxito | Mensaje de éxito | T3 | H3, reprogramar desde Mis citas |
