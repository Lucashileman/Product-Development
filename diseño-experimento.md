# Diseño del experimento — Time-Mirror

## 1. Punto de partida

- Cliente / usuario: estudiantes de Marketing de 2do año, nivel socioeconómico medio-alto, que utilizan redes sociales durante momentos de estudio.
- Problema: los estudiantes tienen dificultades para controlar cuánto tiempo pasan en redes sociales mientras estudian y tienden a subestimar ese tiempo.
- Evidencia obtenida en Clase 4: hubo 8 respuestas medibles. En 6 de ellas, es decir el 75%, la diferencia entre el tiempo que la persona creía haber pasado en redes y el tiempo real fue de 5 minutos o más. Además, los 8 participantes subestimaron su tiempo en alguna medida.
- Hipótesis respaldada: existe una diferencia relevante entre el tiempo percibido y el tiempo real que algunos estudiantes pasan en redes durante una sesión de estudio.
- Limitaciones: la muestra es chica y no representa a todos los estudiantes. Algunos participantes respondieron utilizando rangos en vez de minutos exactos.
- Incertidumbre abierta: todavía no sabemos si mostrarle al estudiante cuánto tiempo lleva realmente en redes es suficiente para que cambie su comportamiento y vuelva a estudiar.
- Decisión del equipo: conservamos el problema validado y avanzamos a probar la hipótesis de valor.

## 2. Pregunta de aprendizaje

¿Cuando un estudiante recibe un aviso que le muestra cuánto tiempo lleva usando una red social durante una sesión de estudio, vuelve a la actividad académica poco tiempo después?

## 3. Hipótesis de valor

Creemos que mostrarle al estudiante, en el momento, cuánto tiempo lleva en redes sociales hará que tome conciencia del desvío y vuelva antes a la actividad académica.

## 4. Alternativas de experimento

### Alternativa A — Wizard of Oz

Funcionamiento: durante una sesión real de estudio, un integrante del equipo detecta manualmente que el participante está usando una red social. Después de 5 minutos le envía un aviso: “Llevás 5 minutos en redes.”

- Acción observada: si deja la red y vuelve a estudiar.
- Dato: cuánto tarda entre recibir el aviso y volver a la tarea.
- Real: estudiante, sesión, uso de redes, aviso y comportamiento.
- Simulado: detección automática y envío automático.
- Costo/dificultad: bajos.
- Calidad de evidencia: alta para esta etapa porque observa comportamiento real.

### Alternativa B — Prototipo navegable

Mostrar una interfaz simulada de Time-Mirror y preguntarle al estudiante qué haría al recibir el aviso.

- Dato: opinión o intención declarada.
- Costo: muy bajo.
- Problema: mide principalmente lo que dice que haría, no lo que efectivamente hace.

### Alternativa C — Extensión funcional

Construir una extensión que detecte automáticamente el uso de redes y envíe el aviso.

- Dato: comportamiento real.
- Costo/dificultad: más altos.
- Problema: implica construir bastante tecnología antes de saber si el mecanismo de aviso genera valor.

## 5. Decisión del equipo

Elegimos la Alternativa A: Wizard of Oz.

Es la alternativa que permite conseguir evidencia de comportamiento real con la menor inversión.

## 6. Contrato experimental

| Campo | Definición |
|---|---|
| Hipótesis | Mostrarle al estudiante cuánto tiempo lleva en redes durante una sesión de estudio hará que vuelva a la tarea poco tiempo después. |
| Aprendizaje | Saber si hacer visible el tiempo transcurrido provoca un cambio observable en su comportamiento. |
| Participantes | 6 estudiantes de Marketing de 2do año. |
| Acción observada | Dejar la red social y volver a la actividad académica después del aviso. |
| Métrica | Tiempo entre el aviso y el regreso a la actividad académica. |
| Criterio | La hipótesis queda respaldada si al menos 4 de 6 participantes vuelven a estudiar dentro de los 2 minutos posteriores al aviso. |
| Duración | Una sesión real por participante; termina después de 6 pruebas válidas. |
| Limitación | No demuestra que usarían Time-Mirror voluntariamente ni que mantendrían su uso a largo plazo. |

## 7. Alcance mínimo

### Imprescindible

- Sesión real de estudio.
- Estudiante real.
- Uso real de una red social.
- Poder medir cuándo empieza a usarla.
- Enviar un aviso.
- Medir cuánto tarda en volver a estudiar.
- Registrar el resultado.

### Simulable

- Detección automática de Instagram/TikTok.
- Conteo automático de tiempo.
- Envío automático del aviso.

Estas funciones pueden ser realizadas manualmente por un integrante del equipo.

### Fuera de alcance

- Login.
- Perfil personal.
- Estadísticas históricas.
- Gamificación.
- Sistema de puntos.
- Bloqueo de aplicaciones.
- Inteligencia artificial.
- Pagos.
- Extensión definitiva.
- App completa.

## 8. Funcionamiento del experimento

- El estudiante comienza a estudiar.
- Entra a una red social.
- El equipo detecta manualmente el ingreso.
- Se cuentan 5 minutos.
- Se envía el aviso: “Llevás 5 minutos en redes.”
- Se mide cuánto tarda el participante en volver a estudiar.
- Se registra el resultado.

## 9. Verificación antes de probar

- Ejecución de principio a fin: el experimento puede realizarse completo.
- Funcionamiento de la medición: se utiliza un cronómetro para medir el tiempo entre el aviso y el regreso a la actividad académica.
- Partes simuladas: detección del uso de redes, conteo automático y envío automático del aviso.
- Parte real: reacción y comportamiento del participante.
- Funciones innecesarias: no se incluyen login, perfiles, estadísticas, gamificación, bloqueos, pagos u otras funciones que no sean necesarias.
- Datos personales: no se registran nombres completos, contraseñas, contenido de mensajes ni información privada del celular.
- Comprensión del equipo: el equipo entiende qué parte es real, cuál es simulada, qué se mide y por qué esa medición permite responder la pregunta de aprendizaje.
