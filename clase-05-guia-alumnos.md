# Clase 5 – Experimentos funcionales: construir para medir

## Propósito

En la Clase 4 reunimos evidencia sobre el cliente y el problema. En esta clase vamos a transformar una incertidumbre abierta en un experimento funcional, rápido, barato y medible.

> **No construimos para lanzar. Construimos para aprender.**

La inteligencia artificial permitirá investigar alternativas, sintetizar información, construir instrumentos y organizar resultados. El equipo deberá interpretar, elegir, controlar y decidir.

> **La IA opera y propone. El equipo piensa y decide.**

---

## Del modelo tradicional al modelo AI-Native

### Modelo tradicional

```text
Cliente
↓
Problema
↓
Idea
↓
MVP
↓
Medir
↓
Aprender
```

Este modelo sigue siendo válido. La IA no lo reemplaza: reduce el tiempo y el costo entre sus etapas.

### Ciclo AI-Native

```text
Cliente
↓
IA ayuda a investigar
↓
Equipo interpreta
↓
IA sintetiza
↓
Equipo decide
↓
IA construye
↓
Usuarios prueban
↓
IA analiza el feedback
↓
Equipo aprende
↓
Nuevo experimento
```

La IA acelera el ciclo. El equipo conserva el criterio, la dirección y la responsabilidad.

---

## Objetivos

Al finalizar, cada equipo podrá:

- identificar una incertidumbre relevante a partir de la evidencia;
- formular una pregunta de aprendizaje observable;
- comparar diferentes tipos de experimentos;
- definir métrica y criterio antes de construir;
- construir con IA un instrumento digital funcional;
- realizar una prueba piloto;
- registrar mediciones, errores y evidencia sin alterarlos;
- reconocer cuándo un experimento dejó de producir aprendizaje;
- iterar o pivotar sin reiniciar el proceso completo;
- dejar preparada la información para aprender y decidir en la Clase 6.

---

## Experimento funcional y MVP

| Experimento funcional | MVP |
|---|---|
| Responde una pregunta | Entrega valor de manera sostenida |
| Puede simular partes | Requiere una experiencia mínimamente completa |
| Debe ser barato y descartable | Supone mayor compromiso e inversión |
| Mide una incertidumbre | Evalúa uso y valor en condiciones más reales |
| Puede vivir pocas horas o días | Debe mantenerse durante un período |

En esta clase no construiremos el MVP. Construiremos un instrumento para producir evidencia.

---

## Entradas

Cada equipo deberá tener disponibles:

- `lean-product-canvas.md`;
- entregable de validación de la Clase 4;
- evidencias originales: notas, entrevistas, observaciones, datos o registros;
- hipótesis e incertidumbres que continúan abiertas.

La Clase 5 no vuelve a investigar el problema desde cero. Parte de lo aprendido y pregunta:

> **¿Qué necesitamos comprobar ahora para reducir la siguiente incertidumbre?**

---

## Uso de la skill

Iniciar una conversación nueva con la skill `ejecutar-experimento-producto` y adjuntar los archivos de entrada.

```text
Quiero diseñar el experimento funcional de la Clase 5.
Leé el Lean Product Canvas y el entregable de validación de la Clase 4.
Guiame paso a paso y hacé una sola pregunta por vez.
Si un experimento deja de producir aprendizaje, no me envíes al inicio
del proceso ni descartes automáticamente el problema. Ayudame a identificar
qué supuesto quedó cuestionado, qué debemos conservar y cuál es el siguiente
experimento más barato para el mismo problema.
```

La skill debe detenerse en las decisiones importantes. No permitan que la IA recorra todo el proceso sin intervención del equipo.

---

## Actividad paso a paso

### Paso 1 – Reconstruir el aprendizaje anterior

Cliente / usuario: Estudiantes de Marketing de 2do año, nivel socioeconómico medio-alto, que utilizan redes sociales durante momentos de estudio.
Problema: Los estudiantes tienen dificultades para controlar cuánto tiempo pasan en redes sociales mientras estudian y tienden a subestimar ese tiempo.
Evidencia obtenida: En el experimento de Clase 4 hubo 8 respuestas medibles. En 6 de ellas, es decir el 75%, la diferencia entre el tiempo que la persona creía haber pasado en redes y el tiempo real fue de 5 minutos o más. Además, los 8 participantes subestimaron su tiempo en alguna medida.    clase-04-guia-alumnos
Hipótesis respaldada: La hipótesis de problema queda respaldada para esta etapa: existe una diferencia relevante entre el tiempo percibido y el tiempo real que algunos estudiantes pasan en redes durante una sesión de estudio.
Contradicciones / limitaciones: La muestra es chica y no representa a todos los estudiantes. Además, algunos participantes respondieron utilizando rangos en vez de minutos exactos, lo que introduce cierto margen de error.    clase-04-guia-alumnos
Incertidumbre abierta: Todavía no sabemos si mostrarle al estudiante cuánto tiempo lleva realmente en redes es suficiente para que cambie su comportamiento y vuelva a estudiar.
Decisión del equipo: conservamos el problema validado y avanzamos a probar la hipótesis de valor.

### Paso 2 – Elegir una pregunta de aprendizaje

Pregunta elegida: ¿Cuando un estudiante recibe un aviso que le muestra cuánto tiempo lleva usando una red social durante una sesión de estudio, vuelve a la actividad académica poco tiempo después?
Hipótesis de valor: Creemos que mostrarle al estudiante, en el momento, cuánto tiempo lleva en redes sociales hará que tome conciencia del desvío y vuelva antes a la actividad académica.

### Paso 3 – Comparar experimentos

Alternativa A — Wizard of Oz
Funcionamiento: Durante una sesión real de estudio, un integrante del equipo detecta manualmente que el participante está usando una red social. Después de 5 minutos le envía un aviso: “Llevás 5 minutos en redes.”

Acción observada: si deja la red y vuelve a estudiar.
Dato: cuánto tarda entre recibir el aviso y volver a la tarea.
Real: estudiante, sesión, uso de redes, aviso y comportamiento.
Simulado: detección automática y envío automático.
Costo/dificultad: bajos.
Calidad de evidencia: alta para esta etapa porque observa comportamiento real.

Alternativa B — Prototipo navegable
Mostrar una interfaz simulada de Time-Mirror y preguntarle al estudiante qué haría al recibir el aviso.
Dato: opinión o intención declarada.
Costo: muy bajo.
Problema: mide principalmente lo que dice que haría, no lo que efectivamente hace.

Alternativa C — Extensión funcional
Construir una extensión que detecte automáticamente el uso de redes y envíe el aviso.
Dato: comportamiento real.
Costo/dificultad: más altos.
Problema: implica construir bastante tecnología antes de saber si el mecanismo de aviso genera valor.

Decisión:
Elegimos la Alternativa A: Wizard of Oz.
Es la alternativa que permite conseguir evidencia de comportamiento real con la menor inversión. Además, Wizard of Oz está expresamente contemplado entre los experimentos posibles de la guía.

### Paso 4 – Definir el contrato experimental

Campo	Definición
Hipótesis	Mostrarle al estudiante cuánto tiempo lleva en redes durante una sesión de estudio hará que vuelva a la tarea poco tiempo después.
Aprendizaje	Saber si hacer visible el tiempo transcurrido provoca un cambio observable en su comportamiento.
Participantes	6 estudiantes de Marketing de 2do año.
Acción observada	Dejar la red social y volver a la actividad académica después del aviso.
Métrica	Tiempo entre el aviso y el regreso a la actividad académica.
Criterio	La hipótesis queda respaldada si al menos 4 de 6 participantes vuelven a estudiar dentro de los 2 minutos posteriores al aviso.
Duración	Una sesión real por participante; termina después de 6 pruebas válidas.
Limitación	No demuestra que usarían Time-Mirror voluntariamente ni que mantendrían su uso a largo plazo.

### Paso 5 – Reducir el alcance

Imprescindible
- Sesión real de estudio.
- Estudiante real.
- Uso real de una red social.
- Poder medir cuándo empieza a usarla.
- Enviar un aviso.
- Medir cuánto tarda en volver a estudiar.
- Registrar el resultado.

Simulable
- Detección automática de Instagram/TikTok.
- Conteo automático de tiempo.
- Envío automático del aviso.
Todo esto lo puede hacer manualmente un integrante del equipo.

Fuera de alcance
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
  
Decisión: Construimos solamente lo necesario para probar si el aviso cambia el comportamiento

### Paso 6 – Construir con IA

La IA puede crear código, notebooks, interfaces, formularios, textos, automatizaciones, datos simulados y mecanismos de registro.

El equipo debe verificar:


Ejecución de principio a fin:	El experimento puede realizarse completo: el estudiante comienza a estudiar, entra a una red social, el equipo mide 5 minutos, envía el aviso y registra cuánto tarda en volver a la tarea.
Funcionamiento de la medición:	La medición se realiza con un cronómetro. Se registra el tiempo entre el momento en que se envía el aviso y el momento en que el participante vuelve a estudiar.
Identificación de partes simuladas:	Se simulan manualmente la detección del uso de redes, el conteo automático del tiempo y el envío automático de la notificación. La reacción del participante es real.
Ausencia de funciones innecesarias:	No se incluyen login, perfiles, estadísticas, gamificación, bloqueos, pagos ni otras funciones que no sean necesarias para probar la hipótesis actual.
Cuidado de datos personales:	No se registran nombres completos, contraseñas, contenido de mensajes ni información privada del celular. Los participantes pueden identificarse como P1, P2, P3, etc.
Comprensión de lo construido:	El equipo entiende qué parte del experimento es real, qué parte está simulada, qué se está midiendo y por qué esa medición permite responder la pregunta de aprendizaje.

### Paso 7 – Realizar el piloto

Se simuló el piloto con 2 estudiantes para verificar si el aviso era claro y si la medición podía realizarse correctamente.

Piloto 1:
- El participante comenzó a estudiar Matemática Financiera.
- A los 18 minutos abrió Instagram.
- Permaneció 5 minutos en la aplicación.
- Se envió el aviso: “Llevás 5 minutos en redes.”
- Cerró Instagram 1 minuto y 10 segundos después.
- Volvió a estudiar inmediatamente.
Observación: el participante entendió el mensaje sin necesidad de explicación adicional.
Piloto 2:
- El participante estaba estudiando Economía.
- Abrió TikTok durante una pausa.
- A los 5 minutos recibió el aviso.
- Continuó usando TikTok durante aproximadamente 3 minutos más.
- Luego dejó el celular y volvió a estudiar.
Observación: el aviso fue visto, pero no produjo una vuelta inmediata a la tarea.
Aprendizajes del piloto simulado:
- El mensaje fue suficientemente claro.
- No fue necesario agregar una orden como “volvé a estudiar”.
- El tiempo entre el aviso y la vuelta a la tarea pudo medirse sin dificultad.
- Se decidió conservar el mensaje original y el criterio de 2 minutos.
- Se agregó una columna para registrar si el participante vio el aviso inmediatamente o después.

### Paso 8 – Ejecutar y registrar

| Participante | Acción observada | Tiempo hasta volver a estudiar | Error / anomalía | ¿Abandonó? | Resultado |
|---|---|---:|---|---|---|
| Benja | Vio el aviso y cerró Instagram | 42 seg | Ninguna | No | Volvió dentro de 2 min |
| Grego | Terminó un video y cerró TikTok | 1 min 18 seg | Ninguna | No | Volvió dentro de 2 min |
| Lucas | Vio el aviso pero siguió scrolleando | 3 min 06 seg | Ninguna | No | No volvió dentro de 2 min |
| Balta | Cerró TikTok y dejó el celular | 51 seg | Ninguna | No | Volvió dentro de 2 min |
| Juan | Miró un último contenido y volvió | 1 min 37 seg | Usó WhatsApp unos segundos antes de volver | No | Volvió dentro de 2 min |
| Rayo | Ignoró inicialmente el aviso | 4 min 12 seg | Interrupción por mensaje de la facultad | No | No volvió dentro de 2 min |

### Paso 9 – Activar el loop de iteración o pivot

El criterio de éxito definido antes del experimento era que al menos 4 de los 6 participantes volvieran a estudiar dentro de los 2 minutos posteriores al aviso. 
4 de los 6 participantes cumplieron ese criterio. Por lo tanto, clasificamos el resultado como: Respaldada por esta prueba simulada.
Los resultados alcanzaron el criterio que habíamos fijado previamente. Esto no significa que todo Time-Mirror esté validada, sino solamente que la hipótesis específica que estábamos probando —que mostrar el tiempo transcurrido puede ayudar a que el estudiante vuelva a estudiar— recibió apoyo dentro de esta simulación.
También observamos que 2 de los 6 participantes continuaron utilizando redes sociales durante más de 2 minutos después del aviso. Esto indica que mostrar el tiempo no necesariamente sería suficiente para todos los usuarios.

1. ¿El experimento produjo evidencia válida?
Si, la prueba permitió observar exactamente el comportamiento que queríamos medir: qué hacía el participante después de recibir el aviso y cuánto tardaba en volver a estudiar.

2. ¿Falló el instrumento o quedó cuestionada la hipótesis?
No identificamos una falla general del instrumento. El mensaje fue claro, pudo medirse el tiempo posterior al aviso y fue posible diferenciar entre participantes que volvieron rápidamente a estudiar y aquellos que continuaron utilizando redes. La hipótesis tampoco quedó contradicha, porque se alcanzó el criterio de éxito establecido.

3. ¿La métrica representaba realmente el comportamiento buscado?
Sí. La métrica principal fue el tiempo transcurrido entre el aviso y el regreso a la actividad académica. Esta métrica representa directamente el comportamiento que queríamos observar, ya que nuestra hipótesis no era si al estudiante “le gustaba” el aviso, sino si después de verlo modificaba efectivamente su conducta.
La métrica complementaria fue la cantidad de participantes que volvieron a estudiar dentro de los 2 minutos.

4. ¿La muestra, el canal y el contexto fueron adecuados?
Para una prueba inicial, la prueba fue diseñada con 6 estudiantes de Marketing de 2do año, que coincide con el segmento trabajado durante el proyecto. El contexto también fue coherente con el problema: sesiones de estudio en las que el participante comenzaba a utilizar una red social recreativamente.
Como limitación, 6 participantes siguen siendo una muestra pequeña y no permiten generalizar el resultado a todos los estudiantes.

5. ¿Repetir exactamente la misma prueba produciría información nueva?
En principio, no. Si siguiéramos haciendo exactamente el mismo experimento con las mismas condiciones, probablemente empezaríamos a repetir información sobre algo que ya recibió una primera señal favorable.
Una muestra real mayor podría aumentar la confianza, pero la incertidumbre más importante después de esta prueba pasa a ser otra: si los estudiantes utilizarían voluntariamente la herramienta.

6. ¿Existe otro experimento más barato o directo para el mismo problema?
Sí. La siguiente incertidumbre puede probarse sin construir una aplicación completa. Podemos utilizar una versión mínima de Time-Mirror en la que el estudiante tenga que decidir voluntariamente si quiere activar una “sesión de estudio”.
Esto permitiría evaluar adopción sin invertir todavía en el desarrollo técnico completo.

Barreras:

Exposición: si las personas realmente vieron la opción o el aviso.
Comprensión: si entendieron qué hacía la herramienta.
Confianza: si se sintieron cómodos utilizándola.
Interés: si entendieron la propuesta pero decidieron no usarla.

Qué conservamos
- El problema validado en la Clase 4.
- El segmento: estudiantes de Marketing de 2do año.
- La idea de hacer visible el tiempo de uso.
- El aviso como posible mecanismo de intervención.
- El aprendizaje de que el aviso podría generar una reacción rápida en algunos usuarios.
Qué cambia:
Cambia la incertidumbre prioritaria.
Ya no necesitamos preguntar primero si el aviso puede provocar una vuelta rápida al estudio.
Ahora necesitamos investigar si los estudiantes elegirían utilizar la herramienta voluntariamente.

Nuestra decicion es: Avanzar al siguiente experimento.

1. ¿Podemos intervenir sobre alguna causa o consecuencia concreta?
Sí. Podemos intervenir sobre la consecuencia de perder la noción del tiempo mostrando al estudiante cuánto tiempo lleva utilizando una red social.

2. ¿Tenemos acceso a los usuarios, actores, datos y permisos necesarios?
Sí. Tenemos acceso a estudiantes del segmento elegido y podemos realizar experimentos simples con ellos sin necesidad de utilizar información personal sensible.

3. ¿Existe una intervención digital compatible con las restricciones del curso?
Sí. Time-Mirror puede plantearse inicialmente como una herramienta digital simple de aviso o seguimiento de tiempo.

4. ¿Podemos probarla con el tiempo, capacidades y recursos disponibles?
Sí. Podemos seguir validando distintas hipótesis mediante experimentos simples antes de construir una aplicación completa.

Conclusión de resolubilidad: El problema continúa siendo resoluble por el equipo dentro del alcance actual, por lo que no necesitamos cambiar de problema ni de segmento.

Decidimos no repetir exactamente el mismo experimento porque la prueba ya alcanzó la cantidad de participantes acordada y produjo una señal suficiente para pasar a otra incertidumbre.
Repetirlo de la misma manera tendría un aprendizaje marginal menor que probar una nueva pregunta.
Además, existe una prueba más directa para la siguiente incertidumbre: observar si los estudiantes deciden activar voluntariamente la herramienta. Por eso dejamos de insistir con el experimento actual y avanzamos.

Proximo experimento elegido:

Lo que busca: ¿Los estudiantes activarían voluntariamente Time-Mirror antes de comenzar una sesión de estudio?

Nueva hipótesis: Creemos que los estudiantes que reconocen el problema activarán voluntariamente Time-Mirror antes de comenzar una sesión de estudio.

Nueva pregunta de aprendizaje: ¿Los estudiantes activan voluntariamente Time-Mirror en situaciones reales de estudio sin que el equipo se los recuerde?

| Campo | Definición |
|---|---|
| Hipótesis | Los estudiantes activarán voluntariamente Time-Mirror antes de estudiar. |
| Aprendizaje | Saber si existe disposición real a iniciar la herramienta sin recordatorios externos. |
| Participantes | 6 estudiantes de Marketing de 2do año. |
| Acción observada | Activar voluntariamente la sesión de estudio. |
| Métrica | Cantidad de sesiones en las que cada participante activa Time-Mirror por cuenta propia. |
| Criterio | Al menos 4 de 6 participantes deben activarlo voluntariamente en 2 o más sesiones durante la prueba. |
| Duración | 3 sesiones de estudio por participante. |
| Limitación | No demuestra todavía uso sostenido de largo plazo ni disposición a pagar. |

Experimento anterior: Wizard of Oz con aviso “Llevás 5 minutos en redes”.

Resultado: respaldada por esta prueba simulada.

Evidencia producida: 4 de 6 participantes volvieron a estudiar dentro de los 2 minutos posteriores al aviso.

Por qué no sirve seguir insistiendo de la misma manera: el experimento ya produjo una señal sobre la hipótesis de valor y repetirlo exactamente igual aportaría poco aprendizaje nuevo.

Supuesto que quedó cuestionado: ninguno quedó directamente contradicho, aunque sigue abierta la duda de si el aviso es suficiente para todos los usuarios.

Qué conservamos: problema, segmento, Time-Mirror y mecanismo de mostrar el tiempo.

Qué modificamos: la incertidumbre prioritaria.

Tipo de cambio: avanzar al siguiente experimento.

Próximo experimento: activación manual voluntaria de Time-Mirror durante varias sesiones.

Qué evidencia diferente esperamos obtener: si los estudiantes realmente deciden utilizar la herramienta sin que alguien se los recuerde.

Nuevo contrato experimental: medir activaciones voluntarias durante 3 sesiones de estudio por participante.

Decicion final del paso 9: A partir de los resultados simulados, decidimos no corregir, no iterar el mismo experimento y no pivotar el problema. Decidimos avanzar al siguiente experimento, conservando el aprendizaje acumulado y pasando de una hipótesis de valor a una hipótesis de comportamiento/adopción.

### Paso 10 – Limitar el loop

El loop no significa experimentar indefinidamente durante la clase.

- Ejecuten una primera prueba completa.
- Si todavía hay tiempo y la siguiente prueba es pequeña, realicen una segunda vuelta.
- Si requiere nuevos participantes, datos o preparación, déjenla diseñada y lista para ejecutar.
- No agreguen funcionalidades para intentar salvar una solución que no produjo evidencia.
- No cambien simultáneamente hipótesis, segmento, canal, métrica e instrumento: después no podrán saber qué generó el nuevo resultado.

La Clase 5 termina cuando el equipo puede explicar:

1. qué aprendió del experimento;
2. por qué corresponde continuar o dejar de insistir;
3. qué supuesto conserva;
4. qué supuesto modifica;
5. cuál es la siguiente prueba más barata.

---

## Ejemplo: estacionamiento universitario

Una incertidumbre posible es si la información anticipada modifica la decisión antes de llegar.

La IA podría proponer:

1. Landing con horarios y solicitud de alerta.
2. Aplicación sencilla con disponibilidad simulada.
3. Chatbot que recomienda un horario o acceso.

Si el equipo elige la aplicación, podría construir solamente:

- selección del horario de llegada;
- disponibilidad simulada;
- una recomendación;
- registro de consulta o acción.

No necesita login, perfil, pagos, reservas reales, sensores ni predicciones avanzadas si no son indispensables para la hipótesis.

Otra hipótesis podría probarse con un modelo sencillo en Google Colab, diez escenarios definidos previamente y un criterio de ocho resultados coherentes sobre diez. Ese experimento produce evidencia técnica, no evidencia de adopción.

---

## Entregables

### 1. Instrumento funcional

Enlace, archivo o instrucciones para ejecutar el experimento.

### 2. `diseno-experimento.md`

Debe documentar evidencia de partida, contrato experimental, experimento elegido, partes reales y simuladas, alcance mínimo, protocolo y decisiones humanas.

### 3. `registro-experimento.md`

Debe conservar resultados iniciales, mediciones, errores, anomalías, observaciones y evidencias complementarias.

### 4. Registro de iteraciones y pivots

Si el equipo corrige, itera o pivota, debe agregar al mismo registro:

- por qué dejó de insistir con el experimento anterior;
- qué supuesto quedó cuestionado;
- qué parte del problema y del Canvas conserva;
- qué cambió y en qué nivel;
- alternativas propuestas por la IA;
- decisión tomada por el equipo;
- contrato del siguiente experimento.

No creen un proyecto nuevo ni eliminen los resultados anteriores. El historial de iteraciones forma parte del entregable.

La interpretación final se realizará en la Clase 6. Si el equipo ya formula una lectura inicial, debe separarla claramente de la evidencia.

---

## Criterios de revisión

- [ ] El experimento parte de evidencia de la Clase 4.
- [ ] Trabaja una sola incertidumbre relevante.
- [ ] Permite observar una acción o resultado.
- [ ] La métrica y el criterio se definieron antes de probar.
- [ ] El instrumento funciona de principio a fin.
- [ ] La medición queda registrada.
- [ ] Las simulaciones están identificadas.
- [ ] El alcance es mínimo.
- [ ] La IA propuso y construyó; el equipo evaluó y decidió.
- [ ] Los errores y resultados negativos se conservaron.
- [ ] El equipo distinguió entre corregir, iterar y pivotar.
- [ ] Si dejó de insistir, explicó por qué repetir no produciría información nueva.
- [ ] La siguiente prueba conserva el problema o justifica explícitamente su revisión.
- [ ] El historial de experimentos anteriores permanece visible.
- [ ] No se inventó evidencia.
- [ ] El resultado puede analizarse en la Clase 6.

---

## Cierre

La velocidad no surge de adivinar mejor. Surge de disminuir el costo de estar equivocados y aumentar la frecuencia con la que aprendemos.

> **El mejor experimento no es el más impresionante. Es el que produce evidencia útil con la menor inversión.**

La Clase 5 termina con un experimento funcional, mediciones registradas y una decisión de continuidad. Si el resultado requiere otra vuelta, el nuevo experimento queda ejecutado o diseñado sin reiniciar el proceso. La Clase 6 comenzará preguntando:

> **¿Qué aprendimos y cuál es la próxima iteración más barata?**

> **Cada experimento termina. El aprendizaje continúa.**
