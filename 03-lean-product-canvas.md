# Lean Product Canvas — Descubrimiento de fricciones en el estudio por uso de redes sociales

> Este canvas contiene hipótesis a validar. Las entrevistas reales del Plan de la Clase 2 todavía están pendientes de ejecutar; el contenido de este documento se completó como ejercicio de práctica y se irá ajustando con la evidencia que surja de las entrevistas y del experimento mínimo.

## 1. Problema de negocio

Los estudiantes de Marketing de 2do año, nivel socioeconómico medio-alto, tienen dificultades para sostener su tiempo de estudio planeado cuando usan redes sociales de forma recreativa en momentos de exigencia académica (previo a entregas o parciales), lo que reduce su tiempo efectivo de estudio y podría afectar su desempeño o bienestar académico.

Lo sabemos por dos estudios formales que muestran esta correlación en poblaciones fuera de Argentina (825 y 100 estudiantes).

Todavía necesitamos comprobar si este patrón se repite en nuestro contexto y si la consecuencia relevante es académica (notas, entregas) o de bienestar (estrés, sueño), dado que un estudio de Kansas encontró que este tipo de procrastinación no afecta las notas.

## 2. Resultados de negocio

Reducir el tiempo perdido en scrolleo no planeado durante sesiones de estudio, desde pendiente de medir hasta una reducción notable, en un plazo a definir tras ejecutar el experimento mínimo.

Todavía no contamos con una línea de base — este valor debe obtenerse del experimento (por ejemplo, comparando tiempo percibido vs. tiempo real de uso, o autorreporte antes/después de usar el prototipo).

## 3. Usuarios y clientes

**Usuario = Cliente = Decisor:** el propio estudiante de Marketing, 2do año, nivel socioeconómico medio-alto. Es quien experimentaría el problema, quien usaría la solución y quien decidiría adoptarla (escenario típico de una app gratuita de uso individual, sin un pagador institucional).

**Influenciador:** pendiente de investigar — no identificado con evidencia de la Clase 2. Podrían ser docentes o compañeros de curso, pero es una hipótesis del equipo, no un hallazgo.

Esto asume que no existe un cliente institucional (facultad, cátedra) dispuesto a pagar o promover la solución — habría que confirmarlo si en algún momento se piensa en un modelo de negocio más allá del uso individual gratuito.

## 4. Necesidades y resultados del usuario

Cuando me propongo estudiar o avanzar con una entrega, especialmente con un parcial o entrega cerca, quiero notar cuando me estoy desviando hacia el celular, para poder volver a la tarea a tiempo y proteger mi tiempo de estudio planeado sin llegar con apuro o sacrificando la calidad del trabajo.

Esta redacción asume que el problema principal es "no darse cuenta a tiempo del desvío". Es posible que, en la práctica, la persona sí se dé cuenta pero le cueste volver a la tarea por otros motivos (falta de motivación, la tarea le genera ansiedad, etc.) — algo que habría que diferenciar en las entrevistas.

## 5. Ideas de solución

### Time-Mirror

- **Propuesta:** Una extensión de navegador o app que detecta cuándo el usuario abre una red social durante una "sesión de estudio" que él mismo activó, y le muestra en tiempo real cuánto tiempo lleva ahí (aviso visual suave, no un bloqueo).
- **Valor para el usuario:** le da visibilidad sobre el desvío en el momento en que ocurre, en vez de descubrirlo recién después (conecta con la necesidad de la Caja 4: "notar el desvío a tiempo").
- **Tecnología central:** tracking de tiempo de uso por app/sitio + notificaciones locales.
- **Datos necesarios:** eventos de apertura/cierre de apps o pestañas, timestamp de inicio de la "sesión de estudio" que el usuario activa voluntariamente.
- **Riesgo principal:** que la persona vea el aviso y lo ignore igual — la solución da información, pero no resuelve la falta de motivación para volver a la tarea (esto conecta con la incertidumbre marcada en la Caja 4).
- **Prototipo inicial:** app simple con temporizador manual + notificación tipo "llevás 8 min acá", armada como mockup en Figma o como extensión mínima de Chrome que cuenta tiempo en dominios definidos (ej. instagram.com, tiktok.com).
- **Dependencias:** ninguna dependencia institucional o física; requiere permisos del navegador/sistema operativo para medir tiempo de uso.
- **Estado:** idea no validada.

## 6. Hipótesis principales

**Hipótesis de problema**
Creemos que los estudiantes de Marketing de 2do año no notan cuánto tiempo llevan en redes sociales una vez que se desvían de una sesión de estudio planeada. Lo sabremos si, en entrevistas o en la observación del experimento, más de la mitad de los participantes subestima significativamente el tiempo real transcurrido.

**Hipótesis de valor**
Creemos que mostrarle al usuario, en tiempo real, cuánto tiempo lleva en una red social durante una sesión de estudio lo ayudará a volver antes a la tarea. Lo sabremos si, al usar el prototipo, los participantes reportan haber vuelto a estudiar más rápido que en sesiones sin el aviso.

**Hipótesis de comportamiento**
Creemos que los estudiantes van a activar voluntariamente el modo "sesión de estudio" antes de ponerse a estudiar. Lo sabremos si, al ofrecerles el prototipo, una proporción relevante (a definir) lo activa sin que se lo pidamos explícitamente cada vez.

**Hipótesis de factibilidad**
Creemos que podemos medir de forma confiable cuánto tiempo pasa un usuario en una red social específica mientras tiene activa una "sesión de estudio", usando solo herramientas de navegador (sin acceso a nivel de sistema operativo). Lo sabremos si logramos construir una prueba técnica (extensión de Chrome) que registre correctamente tiempos de entrada y salida a dominios definidos.

## 7. Lo más importante por aprender

| Hipótesis | Incertidumbre 1–5 | Impacto 1–5 | Prioridad | Justificación |
|---|---|---|---|---|
| Problema | 3 | 5 | 1 | Tenemos evidencia indirecta (estudios, blogs) de que la distorsión de tiempo existe, pero cero evidencia directa de nuestro grupo. Si el problema no existe como lo planteamos, toda la propuesta se cae. |
| Valor | 4 | 4 | 2 | No hay ninguna señal todavía de que "ver el tiempo" ayude a volver a estudiar antes; plausible pero no probado. |
| Comportamiento | 4 | 3 | 3 | Es incierto si activarían el modo manualmente, pero la solución podría ajustarse (ej. detección automática) sin invalidar el problema ni el valor. |
| Factibilidad | 2 | 2 | 4 | Medir tiempo en dominios específicos desde una extensión de navegador es una capacidad técnica bien conocida y de bajo riesgo. |

**Pregunta priorizada:**
¿Los estudiantes de Marketing de 2do año realmente subestiman de forma significativa cuánto tiempo pasan en redes sociales cuando se desvían de una sesión de estudio planeada?

### Pre-mortem

Imaginamos que pasaron 6 meses desde el lanzamiento de "Time-Mirror" y la propuesta fracasó. Estas son las causas posibles identificadas:

| Causa | Qué supuesto falló | Señal temprana | Experimento pequeño para investigarlo |
|---|---|---|---|
| Problema poco relevante | Que la distorsión del tiempo es un problema real y no solo un síntoma de la culpa (Problema B de la Clase 2) | En las entrevistas, cada vez que alguien menciona "no me di cuenta del tiempo", enseguida habla de culpa, nunca del tiempo en sí como molestia aislada | El experimento mínimo de la Caja 8 — comparar autorreporte vs. tiempo real |
| Falta de valor para el usuario | Que mostrar el tiempo en tiempo real ayuda a volver a estudiar | Usuarios ven el aviso ("llevás 8 min acá") y lo cierran sin volver a la tarea | Prototipo tipo Wizard of Oz: un integrante del equipo manda el aviso manualmente a 3-4 personas durante una sesión real y observa qué hacen |
| Baja adopción o uso | Que los estudiantes van a activar voluntariamente el "modo estudio" antes de empezar | Se ofrece el prototipo a un grupo y casi nadie lo activa sin que se lo recuerden | Landing page simple con un botón "Quiero probarlo" — medir cuántos se anotan sin incentivo |
| Datos insuficientes o de mala calidad | Que se puede medir de forma confiable el tiempo en dominios específicos desde el navegador | Al construir la extensión, el tracking falla en apps móviles o no distingue bien "sesión de estudio" de uso normal | Prueba técnica: armar la extensión y probarla en 2-3 dispositivos reales antes de mostrarla a usuarios |
| Limitaciones tecnológicas | Que una extensión de navegador de escritorio es suficiente, sin necesitar acceso al celular | Gran parte del scrolleo ocurre en el celular, no en el navegador de escritorio, y una extensión no cubre ese caso | Preguntar explícitamente en las entrevistas en qué dispositivo ocurre el scrolleo durante el estudio |
| Privacidad o confianza | Que los estudiantes están cómodos con que una app trackee su tiempo de uso en apps específicas | En las entrevistas, la gente muestra incomodidad al mencionar la idea de "que algo te mida el tiempo" | Incluir una pregunta directa sobre esto en el guion de entrevistas antes de construir nada |
| Modelo de negocio | Que no hace falta un modelo de negocio porque el usuario es también el cliente, usando algo gratuito | Nadie sigue usándolo pasados los primeros días sin un incentivo (ej. gamificación, grupo) | No prioritario en esta etapa — riesgo de más largo plazo |

**Los tres riesgos más importantes seleccionados por el equipo:**

1. **Problema poco relevante** — que la distorsión del tiempo sea síntoma del Problema B (culpa/fatiga) y no un problema aparte. Si esto falla, invalida la base de la solución elegida.
2. **Limitaciones tecnológicas** — que el scrolleo ocurra mayormente en el celular y no en el navegador de escritorio, lo que dejaría a "Time-Mirror" (como extensión de Chrome) sin aplicación práctica.
3. **Falta de valor para el usuario** — que aunque el problema exista, mostrar el tiempo transcurrido no alcance para cambiar el comportamiento de la persona en el momento.

Con estos tres riesgos identificados, la hipótesis priorizada en la Caja 7 (Hipótesis de problema) sigue siendo la correcta: es la que, si falla, hace caer a las otras dos.

## 8. Experimento mínimo

- **Hipótesis que prueba:** Hipótesis de problema
- **Objetivo:** Confirmar si existe una brecha real entre el tiempo que el estudiante cree haber pasado en redes y el tiempo real, durante una sesión de estudio.
- **Tipo de experimento:** Observación + autorreporte comparado con datos reales
- **Herramienta:** Captura de pantalla de tiempo de uso (Screen Time / Digital Wellbeing nativo del celular) + formulario corto
- **Participantes:** 5 a 8 estudiantes de Marketing, 2do año (los mismos perfiles del Plan de entrevistas de la Clase 2, todavía pendiente de ejecutar)
- **Duración:** Una sesión de estudio real de cada participante (no simulada), seguimiento de 3 a 5 días
- **Tarea:** Antes de estudiar, el participante estima cuánto tiempo cree que va a pasar en redes si se distrae. Al terminar, reporta cuánto tiempo cree que pasó, y luego se compara contra el dato real de su pantalla.
- **Datos necesarios:** Estimación previa, autorreporte posterior, dato real de tiempo de pantalla en apps definidas (Instagram, TikTok)
- **Métrica:** Diferencia entre tiempo autorreportado y tiempo real medido
- **Criterio de éxito:** En más de la mitad de los participantes, la diferencia entre lo reportado y lo real es de 5 minutos o más
- **Criterio de fracaso:** La mayoría de los participantes estima con precisión razonable (diferencia menor a 5 minutos) su tiempo real
- **Aprendizaje esperado:** Si el problema existe con esta magnitud, tiene sentido seguir invirtiendo en una solución de tipo "Time-Mirror". Si no, hay que revisar si el problema real es otro (ej. el Problema A original: procrastinación, sin el componente de distorsión de tiempo).
- **Limitaciones:** Muestra chica (5-8 personas), no representativa de toda la carrera; depende de que los participantes reporten con honestidad (riesgo de deseabilidad social, ya señalado en la Clase 2).

## Cierre del equipo

- **La solución digital que decidimos explorar es:** "Time-Mirror" — una extensión/app que muestra en tiempo real cuánto tiempo lleva el usuario en una red social durante una sesión de estudio activada voluntariamente.
- **La evidencia más fuerte que la respalda es:** los dos estudios de la Clase 2 (825 y 100 estudiantes) que muestran correlación entre uso recreativo de redes y procrastinación académica, más el hallazgo del estudio de Kansas y los relatos de blogs sobre distorsión del tiempo (evidencia débil, marcada como Supuesto).
- **El supuesto más riesgoso es:** que la falta de percepción del tiempo transcurrido (y no solo la falta de motivación para volver a estudiar) es el mecanismo central del problema — todavía no lo confirmamos con entrevistas reales.
- **Lo más importante que necesitamos aprender es:** si los estudiantes de Marketing de 2do año realmente subestiman de forma significativa cuánto tiempo pasan en redes sociales cuando se desvían de una sesión de estudio planeada.
- **El experimento que realizaremos es:** comparar la estimación de tiempo autorreportada por los participantes contra su tiempo real de pantalla, durante una sesión de estudio real.
- **Abandonaremos o cambiaremos la propuesta si:** la mayoría de los participantes estima con precisión razonable (diferencia menor a 5 minutos) el tiempo real que pasaron en redes — en ese caso, el problema de "distorsión de tiempo" perdería sustento y habría que volver a la Caja 1 con el problema de procrastinación en su forma original (sin el componente de "no darse cuenta").
