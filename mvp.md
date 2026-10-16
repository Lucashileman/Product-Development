# Nuestro primer MVP

- Usuario y situación: estudiantes de Marketing de 2do año que utilizan redes sociales durante sus momentos de estudio y pueden perder noción del tiempo que pasan en ellas.

- Valor y acción central: ayudar al estudiante a tomar conciencia del tiempo que lleva usando redes mientras estudia. La acción central es iniciar una sesión de estudio y recibir un aviso luego de 5 minutos en redes.

- Acceso o forma de ejecución: abrir el archivo `time-mirror-mvp-v2.html` en el navegador.

- Recorrido: inicio → empezar sesión de estudio → indicar “Entré a una red social” → comienza el contador de 5 minutos → aparece el aviso → marcar “Volví a estudiar”.

- Funciona / manual o simulado / fuera de alcance:
  - Funciona: inicio de sesión, contador, aviso y registro de vuelta al estudio.
  - Manual: el usuario debe indicar cuándo entra a una red social.
  - Fuera de alcance: detección automática de Instagram o TikTok, login, perfiles, estadísticas, gamificación, pagos e integraciones.

- Evidencia disponible y duda pendiente: el experimento anterior mostró que 4 de 6 participantes volvieron a estudiar dentro de los 2 minutos posteriores al aviso. Todavía no sabemos si los estudiantes usarían voluntariamente Time-Mirror de manera sostenida.

- Qué medimos: si el usuario completa el recorrido y cuánto tarda en volver a estudiar después del aviso.

## Prueba e iteración

- Quién probó y tarea: una primera prueba del MVP fue realizada recorriendo el flujo completo de uso.

- Qué ocurrió y cómo lo sabemos: la primera versión funcionaba, pero no quedaba claro cuándo había que tocar cada botón ni cómo se relacionaba el contador con cada momento del recorrido.

- Devolución concreta que dimos a la IA: pedimos que el recorrido fuera más claro, mostrando un paso por vez y explicando mejor cuándo empieza el contador y cuándo aparece el aviso.

- Cambio realizado y resultado de la nueva prueba: se creó una segunda versión en la que cada paso aparece de forma secuencial. El recorrido quedó más claro y el contador comienza únicamente después de indicar que se entró a una red social.

- Próximo ajuste: probar la versión con otra persona sin explicarle dónde tocar y observar si puede completar el recorrido por sí sola.
