# Observabilidad aplicada al problema docente con IA

> *La observabilidad no es una propiedad del estudiante. Es una propiedad del sistema de evaluación. Un sistema de evaluación poco observable lo era ya antes de la IA: esta solo hizo la opacidad económicamente accesible y técnicamente trivial.*

## ¿Por qué?

La evaluación académica siempre fue un problema de inferencia: el docente no puede leer directamente el estado cognitivo del estudiante, solo deducirlo a partir de sus salidas: exámenes, trabajos, presentaciones. El sistema funcionaba porque existía una correlación estructural: para producir cierta salida, el estudiante necesitaba poseer el conocimiento o la competencia que esa salida evidenciaba.

La IA rompe esa correlación. Actúa como intermediario que sintetiza salidas de calidad sin que el estado interno exista en el estudiante. El resultado es que la entrega puede ser impecable mientras el aprendizaje es inexistente. Es exactamente el problema del médico que solo mira la radiografía sin explorar al paciente: la imagen puede parecer correcta mientras el problema real queda invisible.

## ¿Qué?

**Observabilidad** es la capacidad del sistema de evaluación para inferir el estado cognitivo real del estudiante, no solo medir sus productos finales.

Un sistema con baja observabilidad evalúa únicamente el resultado entregado. Un sistema con alta observabilidad cruza varias fuentes de señal (el proceso que llevó al resultado, la capacidad de explicarlo, la respuesta ante variaciones no previstas) y puede detectar cuando esas señales no son consistentes entre sí.

La diferencia no es de tecnología. Es de diseño de la evaluación.

## ¿Para qué?

El reencuadre tiene tres consecuencias prácticas:

||||
|-|-|-|
La pregunta deja de ser "¿usó IA?" y pasa a ser "¿puedo inferir su estado cognitivo real?". Esto es relevante porque la primera pregunta no tiene respuesta fiable (los detectores automáticos cometen errores graves) mientras que la segunda sí puede responderse con los instrumentos adecuados.|El diseño de las actividades de evaluación se orienta a aumentar los puntos en los que el proceso del estudiante es visible, en lugar de intentar blindar el producto final contra la IA.|La IA deja de ser necesariamente el adversario. Lo que el estudiante hace con ella (cómo la usa, qué acepta, qué cuestiona y cómo integra sus salidas) es información sobre su estado cognitivo que puede hacerse visible si la evaluación está diseñada para ello.

## ¿Cómo?

### Registrar la progresión, no solo el resultado

Un trabajo entregado sin rastro de su proceso de elaboración es opaco por definición. Cualquier mecanismo que deje huella fechada de las fases intermedias (borradores, esquemas, versiones parciales, historial de edición) convierte el proceso en algo examinable. No como vigilancia, sino como evidencia del trabajo real.

Un historial de repositorio Git en informática, un portafolio con borradores en humanidades, un cuaderno de laboratorio en ciencias: distintos instrumentos, mismo principio.

### Cruzar señales

Un estudiante con conocimiento real mantiene consistencia entre distintas fuentes de señal. La IA produce resultados que raramente sobreviven el cruce:

<div align=center>

| Señal | Qué permite inferir |
|---|---|
| Historial de elaboración o borradores | Progresión real del trabajo en el tiempo |
| Defensa oral o pregunta sobre el trabajo | Capacidad de navegar lo que se entregó |
| Variación de los requisitos en el último momento | Adaptabilidad frente a dependencia de un output fijo |
| Errores cometidos y cómo se resuelven | Modelo mental real, no resultado pulido |

</div>

### Inspección focalizada en discontinuidades

No es viable aplicar el mismo nivel de profundidad a todo. El criterio práctico: cuando un trabajo presenta una discontinuidad respecto al historial del estudiante (calidad muy superior a lo habitual, cambio brusco de registro, ausencia de sus errores habituales) esa discontinuidad es una señal que justifica más puntos de observación. No como acusación, sino como diagnóstico: algo en el sistema requiere más información.

Un profesor que conoce a sus estudiantes reconoce esa discontinuidad sin necesidad de ninguna herramienta. El problema es cuando el volumen o la modalidad hace imposible ese conocimiento directo.

### Consignas que no tienen respuesta genérica

Una consigna con respuesta única y predecible puede ser respondida sin comprensión real. Una consigna anclada al contexto específico del trabajo del propio estudiante ("explica por qué elegiste este enfoque y no el alternativo que descartaste") no tiene respuesta genérica posible, porque requiere el estado interno como condición de posibilidad. La IA puede generar texto sobre ese tema; no puede responder sobre esa decisión concreta, tomada por esa persona, en ese momento.
