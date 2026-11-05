# Conclusiones

1. Pasar de requisitos a wireframes y luego a un prototipo navegable permitió ver fallos que en papel no se notaban, sobre todo en el error de reserva concurrente.
2. Los dos momentos de verdad, elegir la hora (tp4) y confirmar (tp7), son los que más afectan la confianza del paciente; la v2 se enfocó en garantizar recuperación inmediata sin perder datos ya ingresados.
3. El prototipo en HTML permite probar navegación, validación y estados de respuesta con alta fidelidad interactiva, pero no la conexión real con bases de datos ni pasarelas hospitalarias reales.
4. Incidencia sorpresa: El bloque reactivo CONFIG al inicio de `index.html` permite modificar horarios y cupos en segundos durante la defensa, verificando de forma inmediata la resiliencia de la interfaz en rutas normales y de error.
