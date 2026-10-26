# Nuestro primer MVP

- Usuario y situación: estudiantes de Marketing de 2do año que utilizan redes sociales durante sus momentos de estudio y pueden perder noción del tiempo que pasan en ellas.

- Valor y acción central: ayudar al estudiante a tomar conciencia del tiempo que lleva usando redes mientras estudia. La acción central es iniciar una sesión de estudio y recibir un aviso luego de 5 minutos en redes.

- Acceso o forma de ejecución: abrir el archivo `time-mirror-mvp-v3.html` en el navegador.

- Recorrido: inicio → empezar sesión de estudio → indicar “Entré a una red social” → comienza el contador de 5 minutos → aparece el aviso → marcar “Volví a estudiar”.

- Funciona / manual o simulado / fuera de alcance:
  - Funciona: inicio de sesión, contador de 5 minutos, aviso, botón “Volver a estudiar” y registro de vuelta al estudio.
  - Manual: el usuario debe indicar cuándo entra a una red social.
  - Fuera de alcance: detección automática de Instagram o TikTok, login, perfiles, estadísticas, gamificación, pagos e integraciones.

- Evidencia disponible y duda pendiente: en la segunda ronda de prueba con la versión v3, los 5 participantes terminaron volviendo a estudiar y 4 de 5 lo hicieron después del primer aviso. Todavía necesitamos comprobar qué mecanismo puede ayudar a quienes ven el primer aviso pero deciden continuar usando redes.

- Qué medimos: si el usuario completa el recorrido y cuánto tarda en volver a estudiar después del aviso.

## Prueba e iteración

- Quién probó y tarea: un estudiante probó el MVP durante una sesión de estudio. Debía utilizar Time-Mirror mientras estudiaba y seguir el recorrido si entraba a una red social.

- Qué ocurrió y cómo lo sabemos: comenzó su sesión de estudio y luego entró a una red social. Permaneció en ella hasta recibir el aviso de los 5 minutos y, después del aviso, volvió a estudiar.

- Devolución concreta que dimos a la IA: en la primera versión no quedaba claro cuándo tocar cada botón ni cómo se relacionaba el contador con el recorrido. Pedimos mostrar el proceso paso a paso.

- Cambio realizado y resultado de la nueva prueba: se creó una segunda versión más clara, mostrando una acción por vez. El estudiante pudo completar el recorrido sin ayuda y entendió el aviso.

- Próximo ajuste: probar un segundo recordatorio después de 5 minutos adicionales para observar si ayuda a los usuarios que ven el primer aviso pero deciden continuar usando redes.
