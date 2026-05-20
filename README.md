# pyProtocoloIA

La universidad tiene un [protocolo de integridad académica con IA](protocolo/). Son dos documentos que explican por qué la IA es importante, citan el Reglamento EU 2024/1689 y establecen diez ejes de actuación.

Este repositorio intenta ser el aterrizaje del protocolo a algo utilizable.

## El hilo

**El problema no es detectar si el alumno usó IA.** Los detectores automáticos cometen errores graves, van siempre por detrás de los generadores y no responden la pregunta que importa en educación. La pregunta correcta es si el alumno aprendió, es decir, si su estado cognitivo real es inferible a partir de lo que entrega. Eso es un problema de observabilidad del sistema de evaluación, no de vigilancia del estudiante.

**La solución no es tecnológica, es de diseño.** Un sistema de evaluación observable instrumenta el proceso (no solo el producto), cruza varias fuentes de señal y usa consignas que no tienen respuesta genérica. La IA no puede responder "por qué tomaste esta decisión concreta en la sección 3 de tu trabajo". Un alumno que la entiende, sí.

**El protocolo institucional se concreta en cinco acciones para el profesorado**, articuladas en torno a un sistema de cuatro regímenes de uso de IA que se declara en cada enunciado de entrega. Nada más.

**Cada titulación adapta esas cinco acciones** a sus tipos de actividad y a su mecanismo natural de trazabilidad. En Ingeniería Informática ese mecanismo es el historial de commits. En otra titulación será otro artefacto. La plantilla facilita esa conversación.

## Estructura

- Conceptos/
  - [Por que no detección](conceptos/porQueNoDeteccion.md): por qué el protocolo no pivota sobre detectores de IA
  - [Observabilidad](conceptos/observabilidad.md): qué significa hacer observable el proceso cognitivo
- Herramientas/
  - [Verificación oral](herramientas/verificacionOral.md): la pregunta de 5 minutos, la herramienta más potente y universal
  - [Reproducción de escritura](herramientas/reproduccionEscritura.md): herramientas de grabación del proceso de escritura
  - [Consignas ancladas](herramientas/consignasAncladas.md): cómo diseñar enunciados que no tienen respuesta genérica posible
  - [Entrega escalonada](herramientas/entregaEscalonada.md): cómo diseñar hitos intermedios con valor real de trazabilidad
  - [Portafolio de proceso](herramientas/portafolioProceso.md): trazabilidad de autoría para áreas sin mecanismo digital nativo
  - [Repositorio Git](herramientas/repoGitHub.md): el historial de commits como registro de autoría en titulaciones técnicas
  - [Rúbrica de proceso y producto](herramientas/rubricaProceso.md): cómo ponderar evidencia de proceso junto al producto final
- Aterrizajes/
  - [Guion de reunión](aterrizajes/PLANTILLA-guion.md): para facilitar la reunión con el profesorado del área
  - [Pasos explicados](aterrizajes/PLANTILLA-pasos.md): versión autoguiada para leer sin reunión
  - [Formulario por asignatura](aterrizajes/PLANTILLA-aterrizaje.md): el documento que se rellena y queda archivado
  - [II - Ingeniería Informática](aterrizajes/II.md): ejemplo ya resuelto para ese grado
- [protocolo/](protocolo/)
  - Documentos institucionales de referencia

## Orden de lectura

<div align=center>

|||
|-|-|
|**Para entender el marco**|[Por que no deteccion](conceptos/porQueNoDeteccion.md) y luego [observabilidad](conceptos/observabilidad.md).|
|**Para una reunión con profesorado**|[Guion de reunión](aterrizajes/PLANTILLA-guion.md) y el [formulario](aterrizajes/PLANTILLA-aterrizaje.md) en mano.|
|**Para ver un ejemplo resuelto**|[II - Ingeniería Informática](aterrizajes/II.md).|

</div>

Las herramientas son consulta puntual, no lectura previa obligatoria.
