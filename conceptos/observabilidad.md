# Observabilidad aplicada al problema docente con IA

> *La observabilidad no es una propiedad del estudiante. Es una propiedad del **sistema de evaluación**. Un sistema de evaluación poco observable lo era ya antes de la IA: esta solo hizo la opacidad económicamente accesible y técnicamente trivial.*

## ¿Por qué?

> *El desacople output/estado interno*

La evaluación académica siempre fue un problema de observabilidad: el docente no puede leer el estado cognitivo del estudiante directamente, solo inferirlo a partir de sus salidas (exámenes, trabajos, código). El sistema funcionaba porque existía una **correlación estructural** entre la capacidad de producir cierta salida y poseer el estado interno correspondiente.

La IA rompe esa correlación actuando como intermediario que sintetiza salidas sin que el estado interno exista en el estudiante. El sistema se vuelve opaco no porque el estudiante oculte algo, sino porque **el canal de salida ya no es causal respecto al estado que se quiere medir**.

Es exactamente el problema del monitoreo sin observabilidad: la métrica (nota, entrega) puede ser verde mientras el sistema subyacente (aprendizaje) está completamente roto.

## ¿Qué?

> *Reformulación del problema*

El problema no es "detectar trampa" porque se trata de un callejón sin salida: los detectores de IA son fundamentalmente reactivos, tienen tasas de falso positivo inaceptables y la carrera armamentística entre generadores y detectores la ganan los generadores por diseño.

El problema correcto es ***¿cómo hacer observable el proceso cognitivo del estudiante, no solo su output?***

Esto traslada el foco de la salida final al proceso que la produce - exactamente la distinción entre monitoreo y observabilidad.

## ¿Para qué?

> *Consecuencias del reencuadre*

- La pregunta deja de ser "¿usó IA?" y pasa a ser "¿puedo inferir su estado cognitivo real?".
- El diseño de evaluaciones se orienta a **aumentar los puntos de instrumentación del proceso**, no a blindar el output.
- La IA deja de ser el adversario y puede convertirse en parte del proceso visible - lo que el estudiante hace *con* ella es tan informativo como lo que produce.

## ¿Cómo?

> *Instrumentación del proceso*

### Trazabilidad causal (el equivalente al `trace_id`)

El historial de commits en un repositorio público es exactamente esto: cada commit es un span que registra estado parcial, decisión tomada, momento. No se puede fabricar retrospectivamente sin que la anomalía sea detectable (commits todos en la última hora, ausencia de estados intermedios fallidos, saltos de complejidad no explicados por el historial).

Tu pedagogía de repositorios públicos GitHub ya implementa esto. La observabilidad está en el *diff*, no en el resultado final.

### Correlación entre señales

Un sistema observable requiere que múltiples fuentes de señal sean consistentes. Aplicado:

| Señal | Qué instrumenta |
|---|---|
| Repositorio / historial de edición | Proceso temporal |
| Defensa oral o code review en vivo | Capacidad de navegar el propio trabajo |
| Variación incremental de requisitos | Adaptabilidad vs. dependencia de output fijo |
| Errores cometidos y cómo se resuelven | Modelo mental real |

Un estudiante con estado interno real mantiene consistencia entre estas señales. La IA produce outputs que no sobreviven la correlación cruzada: el código entregado existe, la capacidad de explicar una decisión de diseño arbitraria en él, no.

### Tail-based sampling - inspección focalizada en anomalías

No es viable instrumentar todo con el mismo nivel de profundidad. El equivalente educativo: identificar outputs que presentan discontinuidad estadística con el historial del estudiante y aplicar inspección intensiva ahí. No como acusación, sino como señal de que el sistema requiere más puntos de observación.

### Alta cardinalidad en la evaluación

Las preguntas de examen con respuesta única y predecible son el equivalente a las métricas agregadas: pierden la dimensión que importa. Las consignas con alta cardinalidad - "justifica esta decisión de diseño en el contexto específico de tu implementación" - no tienen respuesta genérica sintetizable, porque requieren el estado interno como condición de posibilidad.
