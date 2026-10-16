# Clase 6 — Aprender, decidir y arrancar el MVP

## Guía rápida para alumnos

## Para qué sirve esta clase

Ya hicieron un experimento. Hoy no vamos a analizarlo como una auditoría: vamos a usarlo para decidir qué hacer y empezar a preparar el MVP.

Sólo vamos a responder cuatro preguntas:

1. ¿Qué queríamos comprobar?
2. ¿Qué pasó?
3. ¿Qué aprendimos?
4. ¿Qué hacemos ahora?

> **No importa si el resultado fue bueno o malo. Importa que nos ayude a decidir el próximo paso.**

La IA puede ordenar la información y proponer opciones. El equipo decide.

---

## Lo que necesitan

Tengan a mano:

- **diseno-experimento.md** de la Clase 5;
- **registro-experimento.md** de la Clase 5;
- si los tienen, capturas, notas o resultados complementarios.

No resuman el experimento de memoria. La IA leerá esos archivos y recuperará lo importante. Si sólo tienen uno de los dos, compartan ese.

---

## Entregable

Creen un archivo corto en su repositorio:

~~~
aprendizaje-y-mvp.md
~~~

Debe poder leerse en una pantalla. No agreguen anexos ni tablas extra.

---

## Agenda — 90 minutos

| Momento | Pregunta | Tiempo |
|---|---|---:|
| 1 | La IA recupera qué hicieron | 10 min |
| 2 | ¿Qué pasó? | 20 min |
| 3 | ¿Qué aprendimos? | 20 min |
| 4 | ¿Qué hacemos ahora? | 20 min |
| 5 | ¿Qué MVP vamos a empezar? | 20 min |

---

# 1. La IA recupera qué hicieron

Compartan o adjunten los archivos de Clase 5. Escriban:

~~~text
Leé nuestro diseno-experimento.md y registro-experimento.md.
Recuperá qué queríamos comprobar, cuál era el criterio, qué hicimos y
qué resultados quedaron registrados. Después decinos si estamos listos
para analizar, si falta completar la prueba o si falta ordenar el registro.
No inventes datos.
~~~

La IA debe devolver:

~~~markdown
## Lo que entiendo de su experimento

- Querían comprobar: si mostrarle al estudiante cuánto tiempo lleva usando redes durante una sesión de estudio hace que vuelva más rápido a estudiar.
- El criterio de éxito era: que al menos 4 de 6 participantes volvieran a estudiar dentro de los 2 minutos posteriores al aviso.
- Construyeron o probaron: un experimento Wizard of Oz con el aviso “Llevás 5 minutos en redes”.
- El resultado registrado fue: 4 de 6 participantes volvieron dentro de los 2 minutos.

## Chequeo rápido

- Hipótesis definida antes de probar: SI
- Criterio definido antes de probar: Sí 
- Hay resultados u observaciones: Sí 
- Estado de la iteración: lista para analizar
~~~

Revisen esa síntesis. Corrijan sólo lo que esté mal.

> La IA recupera el recorrido; el equipo confirma que representa lo que realmente hizo.

---

# 2. ¿Qué pasó?

Registren hasta tres hechos. Un hecho es algo que vieron, midieron o registraron; no una explicación.

~~~markdown
## 2. Resultado

| Qué pasó | Cómo lo sabemos |
|---|---|
| 4 de los 6 participantes volvieron a estudiar dentro de los 2 minutos posteriores al aviso. | Los tiempos registrados fueron 42 segundos, 1 minuto 18 segundos, 51 segundos y 1 minuto 37 segundos. |
| 2 de los 6 participantes tardaron más de 2 minutos en volver a estudiar. | Los tiempos registrados fueron 3 minutos 06 segundos y 4 minutos 12 segundos. |
| Ningún participante abandonó completamente la sesión de estudio. | En los 6 casos registrados, los participantes finalmente volvieron a la actividad académica. |

- Resultado frente al criterio: se alcanzó
- Algo que salió distinto de lo esperado: en 2 de los 6 casos el aviso no generó una vuelta rápida a la tarea y los participantes continuaron utilizando redes durante más de 2 minutos.
~~~

## Uso de IA

Pueden pedir:

~~~text
Ordená estos resultados en hasta tres hechos observables.
No inventes datos ni expliques por qué ocurrieron todavía.

[PEGAR RESULTADOS]
~~~

> Si tienen datos simulados o una prueba técnica, indíquenlo. Demuestran que algo puede funcionar, no que los usuarios lo quieran o lo usen.

---

# 3. ¿Qué aprendimos?

Escriban una sola frase que empiece así:

> **Aprendimos que...**

Y otra:

> **Todavía no sabemos si...**

~~~markdown
## 3. Aprendizaje

- Aprendimos que: mostrarle al estudiante cuánto tiempo lleva usando redes durante una sesión de estudio puede ayudar a que vuelva más rápido a la actividad académica, aunque el aviso no genera el mismo efecto en todos los usuarios.
- Todavía no sabemos si: los estudiantes activarían voluntariamente Time-Mirror antes de comenzar a estudiar y lo utilizarían de manera sostenida sin que alguien se los recuerde.
~~~

No busquen una explicación perfecta. Si el resultado no permite concluir, el aprendizaje puede ser simplemente:

> “Todavía no reunimos suficiente evidencia para responder la pregunta.”

Eso también sirve: evita que el equipo tome una decisión basada en una suposición.

---

# 4. ¿Qué hacemos ahora?

Elijan **una** opción:

| Si pasó esto… | Elegimos… |
|---|---|
| La prueba todavía no llegó a la cantidad o tiempo acordado | **Seguir probando** |
| La prueba tuvo un error técnico o una instrucción confusa | **Arreglar la prueba** |
| La prueba ya no puede enseñarnos algo nuevo | **Probar otro camino** |
| La evidencia ya alcanza para continuar | **Avanzar** |

~~~markdown
## 4. Decisión

- Elegimos: Avanzar.
- Porque: El experimento alcanzó el criterio de éxito definido previamente. 4 de los 6 participantes volvieron a estudiar dentro de los 2 minutos posteriores al aviso, por lo que obtuvimos evidencia suficiente para continuar con la siguiente etapa.
- Próximo paso: Empezar a desarrollar una versión mínima de Time-Mirror que permita comprobar si los estudiantes deciden utilizar la herramienta voluntariamente durante sus sesiones de estudio.
~~~

### Si eligen “probar otro camino”

No descarten automáticamente el problema. Cambien primero la forma de resolverlo, el canal, el segmento o el alcance.

> **Cambiar de camino no es empezar de cero. Es conservar lo aprendido y probar algo mejor.**

---

# 5. ¿Qué MVP vamos a empezar?

No diseñen diez pantallas ni una lista de funcionalidades. Definan el valor mínimo que el MVP debe entregar.

~~~markdown
## 5. Punto de partida del MVP

- Usuario: Estudiantes de Marketing de 2do año que utilizan redes sociales durante sus momentos de estudio.
- Situación: El estudiante comienza una sesión de estudio y puede distraerse utilizando redes sociales sin darse cuenta de cuánto tiempo está pasando en ellas.
- Valor que queremos entregar: Ayudar al estudiante a tomar conciencia del tiempo que lleva usando redes mientras estudia para que pueda volver a la actividad académica antes de perder demasiado tiempo.
- Una sola cosa que el MVP debe permitir hacer: Iniciar voluntariamente una sesión de estudio y recibir un aviso que le muestre cuánto tiempo lleva usando redes durante esa sesión.
- Qué vamos a medir cuando lo use una persona: Si el estudiante activa voluntariamente Time-Mirror y, cuando recibe el aviso, cuánto tarda en volver a la actividad académica.
~~~

## Ejemplo: estacionamiento universitario

| Campo | Ejemplo |
|---|---|
| Usuario | Estudiante que llega a primera hora |
| Situación | Sale hacia la universidad sin saber dónde estacionar |
| Valor | Reducir la incertidumbre antes de salir |
| Una cosa que hace el MVP | Muestra disponibilidad estimada para un horario |
| Qué medimos | Si consulta la información y cambia su decisión de llegada |

> **Si una función no entrega este valor o no ayuda a medirlo, no entra en el MVP.**

En la próxima clase vamos a diseñar y construir esta versión mínima.

---

## Entrega

Antes de terminar, revisen:

- [X] La hipótesis y el criterio son los originales.
- [X] Registramos hechos, no explicaciones disfrazadas.
- [X] Escribimos un aprendizaje y una duda que sigue abierta.
- [X] Elegimos un solo próximo paso.
- [X] El MVP tiene un usuario, un valor y una única acción central.

## Cierre

> **El experimento no existe para defender una idea. Existe para que la siguiente versión sea mejor que la primera.**
