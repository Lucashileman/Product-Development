# Clase 8 — Probar, medir y mejorar el MVP con IA

**Desarrollo de Productos · AI-Native Product Development**

## Objetivo de la clase

Observar si una persona puede usar nuestro MVP y obtener el valor que prometemos. Usar evidencia para elegir una mejora, dirigir a la IA para implementarla y volver a medir.

**Pregunta central: ¿el usuario logra resolver la tarea principal con nuestro MVP?**

Venimos de construir una primera versión en la clase 7. Ahora seguimos este ciclo:

**Definir tarea y métricas → probar → registrar → priorizar → mejorar con IA → volver a medir.**

## Qué necesitan para empezar

- El MVP accesible y su archivo `mvp.md` de la clase 7.
- El usuario, problema y valor que buscan ofrecer; pueden recuperar `aprendizaje-y-mvp.md` si necesitan contexto.
- La herramienta de IA con la que ya están trabajando.
- Compañeros de otros equipos o usuarios que puedan probar.
- Un registro simple: una tabla en Markdown o una planilla alcanza.

Si aún no tienen un recorrido funcional, recorten el alcance hasta lograr **una tarea que alguien pueda completar**. La IA los ayuda a destrabarla. No necesitan reiniciar el canvas ni completar todas las funciones imaginadas.

## 1. Reconstruir el recorrido

Completen brevemente:

1. Nuestro usuario tiene el problema de perder noción del tiempo que pasa en redes sociales cuando está estudiando.
2. La hipótesis más riesgosa era que mostrarle cuánto tiempo lleva usando redes podía ayudarlo a volver más rápido a estudiar.
3. Para probarla hicimos un experimento Wizard of Oz y luego construimos un MVP funcional de Time-Mirror.
4. Observamos que en el experimento anterior 4 de 6 participantes volvieron a estudiar dentro de los 2 minutos posteriores al aviso. En la prueba del MVP, el usuario permaneció en redes hasta recibir el aviso de los 5 minutos y después volvió a estudiar.
5. Por eso decidimos avanzar con Time-Mirror y seguir probando su uso con más estudiantes.
6. Nuestro MVP permite iniciar una sesión de estudio, indicar que se entró a una red social, contar 5 minutos, mostrar un aviso y registrar la vuelta al estudio. Todavía necesitamos comprobar si este comportamiento se repite con más usuarios y si usarían la herramienta de forma sostenida.

Abran las evidencias que respaldan las respuestas. Si algo no se probó, márquenlo como pendiente. Pueden pedir a la IA ayuda para ordenar el relato, sin inventar resultados.

## 2. Elegir una tarea principal

Definan una tarea concreta y el resultado que permite considerarla completada.

> Ejemplo ilustrativo: “Llegás a la universidad y querés consultar una zona donde buscar estacionamiento”.

La consigna debe describir el objetivo, sin explicar dónde hacer clic. Antes de probar, acuerden:

- Tarea: “Estás estudiando y en un momento entrás a una red social. Usá Time-Mirror para controlar ese desvío y volver a estudiar.”
- Inicio de la tarea: cuando el participante comienza una sesión de estudio con Time-Mirror.
- Resultado observable: el participante completa el recorrido y vuelve a estudiar luego del aviso.
- Información real: la sesión de estudio, la entrada a una red social y la vuelta al estudio.
- Información manual: el usuario debe indicar en el MVP cuándo entró a una red social.
- Información simulada: la detección automática de Instagram o TikTok no está implementada.
- Qué cuenta como ayuda: cualquier indicación del equipo sobre qué botón tocar, qué paso seguir o cómo continuar el recorrido.
- Fin del intento:
- Éxito: el participante completa el recorrido y vuelve a estudiar.
- Abandono: deja de usar el MVP o no vuelve a la actividad académica.
- El intento termina cuando completa el recorrido o decide abandonar.

**Consultar una recomendación y encontrar estacionamiento son resultados diferentes.** La interfaz puede funcionar sin que todavía hayamos probado el valor en el mundo real.

## 3. Definir tres métricas antes de probar

| Métrica | Cómo medirla | Fuente y momento | Criterio exploratorio | Qué decisión informa
| --- | --- | --- |
| Éxito de la tarea | Participantes que completan / participantes que intentan. | Observación directa durante el primer intento | Al menos 4 de 5 completan | Si el recorrido principal funciona o necesita cambios|
| Autonomía | Participantes que completan sin ayuda / participantes que intentan. | Observación directa durante el primer intento | Al menos 4 de 5 completan sin ayuda | Si las instrucciones y la interacción son claras|
| Valor | Participantes que vuelven a estudiar después del aviso | Observación directa durante la prueba | Al menos 4 de 5 vuelven a estudiar | Si el aviso genera el comportamiento esperado |

- Se cuenta solamente el primer intento de cada participante.
- Los reintentos se registran aparte.
- Los abandonos y fallas se mantienen dentro del registro.
- Si falta un dato, se informa como “no medido”.


## 4. Probar sin enseñar el recorrido

Probamos la versión v2 con 5 participantes. Tres pertenecían al segmento objetivo y dos estaban fuera del segmento.

A todos se les dio la misma consigna: “Estás estudiando y en un momento entrás a una red social. Usá Time-Mirror para controlar ese desvío y volver a estudiar.”

No se les explicó dónde debían tocar ni qué pasos seguir.

### Registro mínimo

| ID | ¿Pertenece al segmento? | Versión | ¿Intentó? | ¿Completó? | ¿Sin ayuda? | Valor y unidad / no medido | Dificultad y ayuda recibida |
| --- | --- | --- | --- | --- | --- | --- | --- |
| U1 | NO | v2 | SI | SI | No medido | Volvió a estudiar a los 3 min 46 seg | Volvió antes del aviso |
| U2 | NO | v2 | SI | SI | No medido | Volvió después del aviso | Necesitó llegar al aviso de los 5 minutos 
| U3 | SI | v2 | SI | SI | No medido | Volvió después del aviso | Permaneció en redes hasta el aviso
| U4 | SI | v2 | SI | SI | No medido | Volvió después del aviso | Permaneció en redes hasta el aviso
| U5 | SI | v2 | SI | SI | No medido | No volvió después del primer aviso | Permaneció en redes después del aviso

Resultados de la primera ronda

- Éxito: 4 de 5 participantes completaron la tarea.
- Autonomía: no medida.
- Valor: 4 de 5 participantes volvieron a estudiar.
- Entre los 3 usuarios del segmento, 2 volvieron después del aviso y 1 continuó utilizando redes.

## 5. Elegir una mejora con evidencia

Hechos observados:

- Los 5 participantes intentaron utilizar el MVP.
- 4 de 5 volvieron a estudiar.
- Un participante fuera del segmento volvió antes de los 5 minutos.
- Los otros 4 llegaron hasta el aviso.
- Entre los 3 participantes del segmento, 2 volvieron después del aviso y 1 permaneció en redes.

Posible causa:

- No podemos saber con certeza por qué uno de los usuarios continuó utilizando redes después del aviso. Una posible causa es que el aviso no hiciera suficientemente clara la acción que se esperaba del usuario, pero esto todavía debía comprobarse.

Mejora priorizada:

- Priorizamos hacer más clara la acción de volver a estudiar después del aviso. Elegimos esta dificultad porque está directamente relacionada con el valor principal de Time-Mirror: ayudar al estudiante a tomar conciencia del tiempo perdido y volver a estudiar.

Alternativas consideradas

- Hacer el aviso más visible.
- Mostrar una acción clara de “Volver a estudiar” junto con el aviso.
- Mostrar un segundo recordatorio si el usuario continúa en redes.

Decisión del equipo: Elegimos la opción 2 porque era un cambio pequeño y directo, sin agregar funciones innecesarias.

## 6. Dirigir la mejora con IA

- Pedido realizado a la IA: “Implementá un botón claro de ‘Volver a estudiar’ que aparezca junto con el aviso de los 5 minutos. Conservá el recorrido actual y el contador. El criterio de aceptación es que el botón aparezca cuando se cumplan los 5 minutos y permita finalizar correctamente la sesión.”
- Cambio realizado: Se creó la versión v3 del MVP. Cuando se cumplen los 5 minutos aparece el aviso junto con el botón “Volver a estudiar”, haciendo más clara la acción que puede realizar el usuario.
- Verificación técnica: Se verificó que:
1. el recorrido comienza correctamente;
2. el contador empieza después de indicar que se entró a una red social;
3. el aviso aparece al cumplirse los 5 minutos;
4. el botón “Volver a estudiar” aparece junto con el aviso;
5. al utilizar el botón, la sesión finaliza correctamente.
La prueba técnica confirma que la función opera correctamente, pero no demuestra por sí sola que la mejora genere mayor valor para los usuarios.


## 7. Volver a probar y comparar

Realizamos una segunda ronda con 5 participantes utilizando la versión v3. Tres participantes pertenecían al segmento y dos estaban fuera del segmento.

| ID | ¿Pertenece al segmento? | Versión | ¿Intentó? | ¿Completó? | ¿Sin ayuda? | Resultado Observado
| --- | --- | --- | --- | --- | --- | --- | --- |
| U1 | NO | v3 | SI | SI | No medido | Llegó a los 5 minutos, vio la opción de volver a estudiar y volvió
| U2 | NO | v3 | SI | SI | No medido | Llegó a los 5 minutos, vio la opción de volver a estudiar y volvió
| U3 | SI | v3 | SI | SI | No medido | Después del aviso de los 5 minutos volvió a estudiar
| U4 | SI | v3 | SI | SI | No medido | Después del aviso de los 5 minutos volvió a estudiar
| U5 | SI | v3 | SI | SI | No medido | Continuó en redes otros 5 minutos y luego volvió a estudiar

Comparacion:

| Metrica | Antes: v2 | Después: v3 | Qué aprendimos y limitaciones
| Éxito | 4 de 5 completaron | 5 de 5 completaron | En la segunda ronda todos completaron el recorrido. La muestra es pequeña y los participantes fueron distintos |
| Autonomía | No medido | No medido| No registramos suficientemente si los participantes necesitaron ayuda |
| Valor | 4 de 5 volvieron a estudiar | 5 de 5 terminaron volviendo; 4 de 5 lo hicieron después del primer aviso | El resultado fue mejor en esta ronda, pero no podemos afirmar que el cambio haya sido la única causa |

Qué aprendimos:

- Los 5 participantes terminaron volviendo a estudiar.
- 4 de 5 volvieron luego del primer aviso.
- Entre los 3 usuarios del segmento, 2 volvieron después del primer aviso y 1 necesitó más tiempo.
- El botón “Volver a estudiar” hace más explícita la acción propuesta por Time-Mirror.
- El aviso no garantiza que todos los estudiantes vuelvan inmediatamente.
- Todavía necesitamos comprobar qué hacer cuando un usuario recibe el aviso pero decide continuar utilizando redes.

Próximo paso: 

Incertidumbre pendiente: qué mecanismo puede ayudar a los usuarios que ven el primer aviso pero deciden seguir utilizando redes.

Acción más barata: probar un segundo recordatorio después de 5 minutos adicionales.

Responsable: equipo de Time-Mirror.

Momento: próxima ronda de prueba con usuarios del segmento.

Qué observar: cuántos usuarios vuelven con el primer aviso y cuántos necesitan un segundo recordatorio.

Decisión según el resultado: si el segundo recordatorio ayuda a los usuarios que ignoran el primero, evaluar incorporarlo a una próxima versión del MVP.
