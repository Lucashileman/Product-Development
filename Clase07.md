# Clase 7 — Del aprendizaje al primer MVP

## Guía para alumnos · 90 minutos

Hoy van a construir una primera versión que una persona pueda usar para obtener un resultado concreto. Van a hacerlo conversando con la IA: dar contexto, acordar qué construir, probar lo recibido y pedir mejoras.

**Objetivo: aprender a dirigir a la IA para construir, probar e iterar un MVP que entregue un valor concreto.**

## Cómo vamos a trabajar con la IA

La clase empieza con una conversación. La IA recupera el documento de Clase 6, propone un recorrido y espera que el equipo lo confirme o ajuste. Recién después de acordar el alcance y los datos, le piden construir. Al recibir la primera versión, la prueban y le dan una devolución para iterar.

**No peguen todos los pedidos juntos. Háganlos uno por uno y respondan a la IA entre pasos.** Si construye de entrada, pídanle: «Antes de construir, revisemos juntos el recorrido y el alcance. Hacenos una pregunta por vez».

## Qué necesitan

- El archivo `aprendizaje-y-mvp.md` de la Clase 6.
- La herramienta de IA con la que van a construir y, si ya existe, acceso al prototipo o código del equipo.
- Una persona que pueda probar la versión al final, aunque sea otro compañero.

Usen la herramienta que tengan disponible. Si permite skills, activen `construir-mvp-con-ia`. Si no, usen los pedidos de esta guía. Si la IA sólo conversa y no construye, pídanle el pedido completo para llevar a una herramienta que sí pueda hacerlo.

## Qué entregan

1. **Una versión accesible del MVP**, por enlace o con instrucciones sencillas para ejecutarla.
2. **Un archivo `mvp.md` breve** en su repositorio, con lo que funciona, la prueba realizada y el siguiente ajuste.

Una versión que usa datos de demostración debe identificarlos. Que funcione técnicamente no demuestra todavía que sea útil para el usuario.

## Recorrido de la clase

| Momento | Qué vamos a lograr | Tiempo |
|---|---|---:|
| 1. Recuperar | Usuario, valor y acción central claros | 10 min |
| 2. Diseñar | Un recorrido de principio a fin | 15 min |
| 3. Recortar | Alcance y datos definidos | 15 min |
| 4. Construir e iterar | Primera versión funcionando | 35 min |
| 5. Probar y registrar | Observaciones y próximo ajuste | 15 min |

## 1. Recuperar el punto de partida

Compartan el archivo de la Clase 6 y escriban:

```text
- Usuario: estudiantes de Marketing de 2do año que utilizan redes sociales durante sus momentos de estudio.
- Situación: el estudiante comienza una sesión de estudio y puede distraerse usando redes sociales sin darse cuenta de cuánto tiempo pasa en ellas.
- Valor: ayudar al estudiante a tomar conciencia del tiempo que lleva usando redes para que pueda volver antes a estudiar.
- Acción central: iniciar una sesión de estudio y recibir un aviso sobre el tiempo que lleva usando redes.
- Decisión de Clase 6: avanzar con una primera versión mínima de Time-Mirror.
- Duda pendiente: si los estudiantes utilizarían Time-Mirror voluntariamente durante sus sesiones de estudio.
- Herramienta elegida: ChatGPT.
```

Corrijan lo que la IA haya entendido mal. No vuelvan a completar el canvas ni a relatar todo el proyecto.

Si todavía falta evidencia, mantengan esa duda explícita. Pueden construir para seguir aprendiendo; no presenten esa construcción como una validación que todavía no ocurrió.

## 2. Diseñar un recorrido mínimo

Pidan:

```text
Inicio → Empezar sesión de estudio → Entré a una red social → comienza un contador de 5 minutos → aparece el aviso “Llevás 5 minutos en redes” → Volví a estudiar.

Criterio de funcionamiento: cuando el usuario indica que entró a una red social, el sistema debe contar 5 minutos y mostrar correctamente el aviso.

Si todavía no comenzó una sesión de estudio, no debe poder iniciar el registro de uso de redes.
```

Revisen: **¿la persona obtiene un resultado útil al terminar?** Decidan con la IA el recorrido que van a construir.

Ejemplo ilustrativo: un estudiante consulta el último reporte por sector y su hora de actualización para decidir a qué sector dirigirse. El criterio técnico es mostrar el reporte disponible o informar claramente que no hay datos. Predecir disponibilidad futura es otro alcance y necesita datos adicionales. Que el reporte ayude a decidir requiere una prueba con una persona.

## 3. Recortar el alcance y resolver los datos

```text
| Categoría | Definición |
|---|---|
| Debe funcionar ahora | Iniciar una sesión de estudio, indicar que entró a una red social, contar 5 minutos, mostrar el aviso y registrar la vuelta al estudio. |
| Manual o simulado | La detección de que el usuario entró a Instagram o TikTok. El usuario lo indica mediante un botón. |
| Fuera de alcance | Detección automática de redes, login, perfiles, estadísticas, gamificación, pagos, bloqueos e integraciones. |

- Datos necesarios: acciones del usuario y tiempos registrados durante la sesión.
- Fuente de los datos: el propio uso del MVP.
```

No hace falta automatizar todo. Una operación manual puede sostener el primer MVP si permite entregar el valor acordado.

En el ejemplo de estacionamiento, ¿quién informa la ocupación y cuándo se actualiza? Si no hay una fuente real, una pantalla con números inventados sólo permite probar el recorrido. Debe mostrar **“Datos de demostración”** y no prometer disponibilidad real.

**Regla de alcance:** si una función no ayuda a completar la acción central o a comprobar su resultado, déjenla para después. Revisen especialmente registro de usuarios, pagos, paneles e integraciones.

## 4. Construir y mejorar conversando con la IA

Cuando el recorrido y el alcance estén claros, escriban:

```text
Construimos con ChatGPT una primera versión funcional de Time-Mirror.

La versión permite:
- empezar una sesión de estudio;
- indicar manualmente que el usuario entró a una red social;
- iniciar un contador de 5 minutos;
- mostrar el aviso “Llevás 5 minutos en redes”;
- registrar cuándo el usuario vuelve a estudiar.

La detección automática de Instagram o TikTok todavía no está incluida, porque para este primer MVP se resolvió de manera manual.
```

Abran la versión y úsenla. No se queden mirando la pantalla ni acepten “listo” como prueba de funcionamiento.

### Cómo darle una devolución útil

Usen cuatro datos: **qué hice, qué esperaba, qué pasó y qué evidencia tengo**.

| Devolución poco útil | Devolución que permite avanzar |
|---|---|
| “No funciona.” | “Elegí el Sector Norte y presioné Consultar. Esperaba ver el último reporte, pero no apareció ningún resultado. Adjunto captura.” |
| “Está feo.” | “El resultado queda debajo de la pantalla y no se ve sin bajar. Mostralo junto al botón de consulta.” |
| “Hacelo mejor.” | “Cuando no hay datos muestra cero lugares. Necesitamos que diga ‘Sin información disponible’.” |

Después pidan:

```text
Primera versión:
Se construyó una primera versión funcional de Time-Mirror en HTML.

Problema detectado:
Al probarla, no quedaba suficientemente claro cuándo había que tocar cada botón ni cómo se relacionaba el contador con cada momento del recorrido.

Devolución concreta a la IA:
“Al probar el MVP, no se entiende bien cuándo hay que tocar cada botón ni cómo se relaciona el tiempo con cada acción. Queremos que el recorrido se muestre paso a paso y que quede claro cuándo empieza el contador y cuándo aparece el aviso.”

Corrección realizada:
Se modificó el MVP para mostrar un solo paso por vez:
1. Empezar sesión de estudio.
2. Indicar que entró a una red social.
3. Mostrar el contador de 5 minutos.
4. Mostrar el aviso.
5. Marcar que volvió a estudiar.

También se agregaron textos explicativos para indicar qué debe hacer el usuario en cada momento.

Cómo comprobamos el cambio:
Abrimos la nueva versión y repetimos el recorrido completo. Verificamos que cada acción aparezca en el orden correcto y que el contador empiece únicamente después de marcar “Entré a una red social”.
```

Vuelvan a probar. Trabajen sobre una prioridad por vez. Si la IA agrega algo innecesario, pregunten: **“¿Esto ayuda a completar la acción central que acordamos?”**

Si cambian de herramienta o conversación, lleven el contexto, la versión actual y el problema concreto. Nunca compartan contraseñas ni claves dentro del pedido.

## 5. Probar con otra persona y registrar

Den una tarea, por ejemplo: “Estás por salir hacia la universidad. Usá esta versión para consultar la información y decidir a qué sector irías”. No le indiquen dónde tocar.

Observen:

- ¿Pudo completar la acción? ¿Necesitó ayuda?
- ¿Entendió el resultado y sus limitaciones?
- ¿Qué hizo con la información? ¿Qué obstáculo encontraron?

Registren intentos y acciones completadas, aunque sea manualmente. Para explorar el valor, observen qué resultado obtuvo la persona; un clic por sí solo no lo demuestra. Identifiquen si probó un compañero o alguien del segmento objetivo. Si no hubo prueba, déjenla pendiente.

Pueden pedirle a la IA:

```text
- Problemas de funcionamiento: no se detectaron problemas técnicos durante la prueba.
- Dificultades de uso: el usuario pudo completar el recorrido sin ayuda y entendió cuándo debía volver a estudiar.
- Dudas sobre el valor: todavía no sabemos si el aviso tendría el mismo efecto en más usuarios ni si usarían Time-Mirror de manera sostenida.
- Próximo ajuste: seguir probando el MVP con más estudiantes y registrar cuánto tardan en volver a estudiar después del aviso.
```

Decidan el ajuste. Si queda tiempo, impleméntenlo y vuelvan a probarlo.

## Plantilla del entregable: mvp.md

Completen con ayuda de la IA. Manténganlo breve; no hace falta copiar toda la conversación.

```markdown
# Nuestro primer MVP
- Usuario y situación: estudiantes de Marketing de 2do año que utilizan redes sociales durante sus momentos de estudio y pueden perder noción del tiempo que pasan en ellas.
- Valor y acción central: ayudar al estudiante a tomar conciencia del tiempo que lleva usando redes mientras estudia. La acción central es iniciar una sesión de estudio y recibir un aviso luego de 5 minutos en redes.
- Acceso o forma de ejecución: abrir el archivo `time-mirror-mvp-v2.html` en el navegador.
- Recorrido: empezar sesión de estudio → indicar “Entré a una red social” → comienza el contador de 5 minutos → aparece el aviso → marcar “Volví a estudiar”.
- Funciona / manual o simulado / fuera de alcance: funciona el inicio de sesión, el contador, el aviso y el registro de vuelta al estudio. La detección de entrada a redes es manual. Quedan fuera de alcance la detección automática, login, perfiles, estadísticas, gamificación, pagos e integraciones.
- Evidencia disponible y duda pendiente: en la prueba realizada, el usuario permaneció en redes hasta recibir el aviso de los 5 minutos y luego volvió a estudiar. Todavía no sabemos si este comportamiento se repetiría con más usuarios ni si utilizarían la herramienta de forma sostenida.
- Qué medimos: si el usuario completa el recorrido, si vuelve a estudiar después del aviso y cuánto tarda en hacerlo.

## Prueba e iteración
- Quién probó (rol) y tarea: Santos Alvarado probó el MVP durante una sesión de estudio. La tarea fue utilizar Time-Mirror mientras estudiaba y, si entraba a una red social, seguir el recorrido del MVP hasta volver a estudiar.
- Qué ocurrió y cómo lo sabemos: comenzó su sesión de estudio y, después de un tiempo, entró a una red social. No volvió a estudiar por su cuenta antes de los 5 minutos. Al cumplirse ese tiempo recibió el aviso y, luego de verlo, volvió a su sesión de estudio.
- ¿Pudo completar la acción sin ayuda?: Sí.
- ¿Entendió el resultado y sus limitaciones?: Sí. Entendió el aviso y lo utilizó como señal para volver a estudiar.
- Obstáculo encontrado: no se observó un problema de funcionamiento durante esta prueba. El usuario permaneció en redes hasta recibir el aviso.
- Devolución concreta: el aviso fue útil como recordatorio para cortar el uso de redes y volver a estudiar.
- Próximo ajuste: seguir probando el MVP con más personas para observar si el mismo comportamiento se repite y registrar cuánto tardan en volver a estudiar después del aviso.
```

## Antes de entregar

- [X] Podemos acceder a la versión y completar la acción central.
- [X] Sabemos qué funciona y qué depende de operación manual o simulación.
- [X] Probamos el recorrido principal y qué ocurre cuando faltan datos o la entrada es inválida.
- [X] Registramos una devolución concreta a la IA y qué pasó después, o marcamos lo pendiente.
- [X] Registramos la prueba con otra persona o la dejamos explícitamente pendiente.
- [X] Conservamos una duda sobre el valor y elegimos el próximo ajuste.

**La IA propone y construye. El equipo dirige, prueba y decide.** En la próxima clase vamos a mejorar esta versión usando lo que observemos al utilizarla.
