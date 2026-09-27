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
| P1 | Vio el aviso y cerró Instagram | 42 seg | Ninguna | No | Volvió dentro de 2 min |
| P2 | Terminó un video y cerró TikTok | 1 min 18 seg | Ninguna | No | Volvió dentro de 2 min |
| P3 | Vio el aviso pero siguió scrolleando | 3 min 06 seg | Ninguna | No | No volvió dentro de 2 min |
| P4 | Cerró TikTok y dejó el celular | 51 seg | Ninguna | No | Volvió dentro de 2 min |
| P5 | Miró un último contenido y volvió | 1 min 37 seg | Usó WhatsApp unos segundos antes de volver | No | Volvió dentro de 2 min |
| P6 | Ignoró inicialmente el aviso | 4 min 12 seg | Interrupción por mensaje de la facultad | No | No volvió dentro de 2 min |

### Paso 9 – Activar el loop de iteración o pivot

Un experimento no debe repetirse solamente porque el resultado no fue favorable. Antes de insistir, el equipo debe identificar **qué dejó de funcionar como supuesto** y si otra prueba puede producir evidencia diferente.

> **No volvemos al comienzo. Volvemos al supuesto que la evidencia puso en duda.**

La IA debe comparar los resultados con el contrato experimental y clasificar el estado:

- **Respaldada por esta prueba:** alcanzó el criterio definido.
- **No respaldada por esta prueba:** produjo evidencia válida, pero no alcanzó el criterio.
- **Inconclusa:** la ejecución o los datos no permiten comparar el resultado con el criterio.

Esta clasificación no autoriza a descartar automáticamente el problema ni toda la solución.

#### Diagnosticar antes de cambiar

La IA debe hacer estas preguntas de a una y esperar la respuesta del equipo:

1. ¿El experimento produjo evidencia válida?
2. ¿Falló el instrumento o quedó cuestionada la hipótesis?
3. ¿La métrica representaba realmente el comportamiento buscado?
4. ¿La muestra, el canal y el contexto fueron adecuados?
5. ¿Repetir exactamente la misma prueba produciría información nueva?
6. ¿Existe otro experimento más barato o directo para el mismo problema?

#### Si nadie realiza la acción

Un resultado como **cero clics, cero aperturas o cero respuestas** no explica por sí solo por qué falló la prueba. Únicamente permite afirmar que, con ese mensaje, canal, contexto y mecanismo, no se observó el comportamiento esperado.

Antes de cambiar el problema, la IA debe ayudar al equipo a distinguir estas barreras, una por vez y sin inventar motivaciones:

| Barrera posible | Evidencia necesaria | Próxima prueba posible |
|---|---|---|
| Exposición | ¿Las personas realmente recibieron o vieron el estímulo? | Verificar alcance o probar otro canal |
| Comprensión | ¿Entendieron qué se les proponía y qué podían hacer? | Prueba moderada de comprensión |
| Confianza | ¿El mensaje y el actor resultaron creíbles? | Wizard of Oz conversacional o prueba de credibilidad |
| Interés | ¿Comprendieron y confiaron, pero decidieron no actuar? | Probar otro mecanismo de valor para el mismo problema |

No repetir el mismo *fake door* hasta identificar qué evidencia nueva produciría la repetición.

#### Elegir el nivel correcto de cambio

| Situación encontrada | Qué se conserva | Qué se cambia | Decisión |
|---|---|---|---|
| Error técnico, tarea confusa o medición defectuosa | Problema, hipótesis y criterio | Instrumento | **Corregir y repetir** |
| Evidencia insuficiente o contexto poco representativo | Problema e hipótesis | Método, muestra, canal o contexto | **Iterar el experimento** |
| Evidencia válida contradice la hipótesis probada | Problema respaldado | Hipótesis de valor, comportamiento, solución o mecanismo | **Pivotar** |
| Evidencia respalda la hipótesis | Aprendizaje acumulado | Incertidumbre prioritaria | **Avanzar al siguiente experimento** |
| Varias pruebas contradicen la existencia o relevancia del problema | Evidencia y trazabilidad | Segmento o formulación del problema | **Actualizar el Canvas** |

> **Cambiar solamente el instrumento es iterar. Cambiar una hipótesis, solución, mecanismo o segmento es pivotar.**

El comportamiento por defecto será conservar el problema validado y buscar otra forma de reducir la incertidumbre. No se vuelve a la Clase 1: el Lean Product Canvas se actualiza en el mismo punto del recorrido y conserva el historial.

#### Control de resolubilidad

Un problema puede existir y ser relevante, pero no resultar abordable por el equipo dentro del alcance del laboratorio. Antes de forzar una solución, responder:

1. ¿Podemos intervenir sobre alguna causa o consecuencia concreta?
2. ¿Tenemos acceso a los usuarios, actores, datos y permisos necesarios?
3. ¿Existe una intervención digital compatible con las restricciones del curso?
4. ¿Podemos probarla con el tiempo, capacidades y recursos disponibles?

Si las respuestas son negativas, registrar:

> **El problema continúa respaldado, pero no es resoluble por este equipo dentro del alcance actual.**

La IA debe proponer estas salidas y esperar la decisión humana:

| Salida | Qué se conserva | Qué cambia |
|---|---|---|
| Cambiar el mecanismo | Problema y segmento | Forma de intervención |
| Reducir el alcance | Problema general | Parte abordada |
| Cambiar usuario o actor | Problema general | Persona capaz de actuar o decidir |
| Pivotar el problema | Dominio y aprendizajes | Oportunidad seleccionada |
| Cerrar el proyecto | Evidencia y trazabilidad | No continúa la construcción |

Si se pivota el problema, volver a las oportunidades de la Clase 2 mediante una **ruta rápida**: seleccionar la nueva oportunidad, actualizar la hipótesis y revisar sólo las partes afectadas del Canvas. No repetir mecánicamente todo el curso.

#### Cuándo dejar de insistir

Detengan el experimento actual cuando:

- alcanzó la cantidad de participantes, escenarios o ejecuciones acordada;
- repite resultados sin agregar información nueva;
- la métrica no representa el comportamiento buscado;
- depende de condiciones que el equipo no puede obtener;
- el costo de repetir supera el aprendizaje esperado;
- otra prueba puede responder la pregunta de forma más directa o barata.

> **Repetir sin producir información nueva no es perseverar: es dejar de aprender.**

#### Diseñar la siguiente prueba

La IA debe proponer entre dos y tres próximos experimentos para el mismo problema. Para cada uno indicará:

- qué supuesto específico pone a prueba;
- qué cambia respecto del experimento anterior;
- qué evidencia nueva podría producir;
- tiempo, costo y dificultad;
- qué resultado obligaría a revisar nuevamente la hipótesis.

Después recomendará la alternativa más barata que pueda generar aprendizaje diferente y se detendrá para que el equipo decida.

**Decisión humana:** continuar, corregir, iterar, pivotar o actualizar el problema.

#### Registro obligatorio del loop

```markdown
## Iteración [NÚMERO]

- Experimento anterior:
- Resultado: respaldada, no respaldada o inconclusa:
- Evidencia producida:
- Por qué no sirve seguir insistiendo de la misma manera:
- Supuesto que quedó cuestionado:
- Qué conservamos:
- Qué modificamos:
- Tipo de cambio: corrección, iteración o pivot:
- Próximo experimento:
- Qué evidencia diferente esperamos obtener:
- Nuevo contrato experimental:
```

No borren ni reescriban el resultado anterior. Cada vuelta debe conservarse para mostrar cómo evolucionó el razonamiento.

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
