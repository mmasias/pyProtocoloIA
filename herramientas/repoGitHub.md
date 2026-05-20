# Repositorio Git como trazabilidad de autoría

## ¿Por qué?

En titulaciones donde el código es el producto, el historial de commits es el rastro natural del proceso de elaboración. No requiere ningún artefacto adicional: el estudiante ya trabaja con Git, y ese trabajo deja una huella fechada, ordenada y verificable de cómo evolucionó el proyecto.

El problema es que ese rastro existe pero raramente se usa como evidencia de autoría. Se entrega el repositorio como contenedor del código, no como registro del proceso.

## ¿Qué?

Un repositorio Git con historial de commits recoge, para cada unidad de cambio: qué se modificó, cuándo, con qué mensaje y bajo qué autoría. Esa secuencia es una reconstrucción cronológica del proceso de elaboración: cuándo empezó el trabajo real, cómo progresó, dónde se concentró el esfuerzo y cómo se resolvieron los problemas.

Usado como herramienta de trazabilidad, el repositorio no es solo el lugar donde vive el código. Es la evidencia de que ese código tiene una historia.

## ¿Para qué?

<div align=center>

| Trazabilidad de autoría | Verificación de proceso | Señal de discontinuidad | Disuasión |
|-|-|-|-|
| El historial con fechas acredita que el trabajo se elaboró progresivamente. Un proyecto entregado con un único commit o con todos los commits en las horas previas a la entrega es una señal inequívoca. | La secuencia de commits permite reconstruir cómo se abordó el problema: orden de implementación, decisiones de diseño, correcciones sobre la marcha. | Un salto brusco de calidad entre commits, la aparición de código sin historia previa o un cambio radical de estilo son discontinuidades observables sin herramientas adicionales. | El conocimiento previo de que el historial se revisará cambia cómo el estudiante gestiona el repositorio durante la elaboración. |

</div>

## ¿Cómo?

### Qué pedir al estudiante

Tres requisitos mínimos que convierten el repositorio en evidencia útil:

- **Commits frecuentes y atómicos:** cada commit recoge una unidad lógica de trabajo, no la entrega final de golpe. Orientativamente, varios commits por sesión de trabajo.
- **Mensajes descriptivos:** el mensaje del commit describe qué se hizo y, cuando proceda, por qué. "fix bug" no aporta información; "corrige desbordamiento en el parser al procesar entradas vacías" sí.
- **Autoría correcta:** el nombre y el correo configurados en Git deben corresponder al estudiante. En trabajos en grupo, los commits individuales identifican la contribución de cada miembro.

### Qué mirar en el historial

| Señal | Qué indica |
|---|---|
| Commits distribuidos a lo largo del período de la actividad | Trabajo progresivo real |
| Commits concentrados en las últimas horas antes de la entrega | Elaboración de último momento o importación de código externo |
| Mensajes vacíos, genéricos o incoherentes con el diff | El historial se creó para cumplir el requisito, no como registro real del trabajo |
| Cambio brusco de estilo o calidad entre commits | Posible incorporación de código de origen distinto |
| Un único commit con todo el proyecto | Ausencia de historial real, independientemente del contenido |

### Cómo solicitarlo

Incluir en el enunciado de la actividad:

- La URL del repositorio como parte de la entrega.
- El requisito explícito de commits frecuentes con mensajes descriptivos.
- La advertencia de que el historial forma parte de la evaluación.

Sin esa advertencia explícita, el estudiante no sabe que el historial importa y no lo cuida.

### Plataformas y acceso

| Plataforma | Acceso para el docente |
|---|---|
| GitHub | Repositorio público o invitación como colaborador |
| GitLab | Mismo modelo que GitHub |
| Bitbucket | Mismo modelo que GitHub |
| Repositorio local entregado | `git log --oneline` o `git log --stat` para revisar el historial |

Para revisar el historial sin clonar el repositorio, GitHub y GitLab muestran el log completo en la interfaz web bajo la pestaña "Commits".

### Límites de la herramienta

El historial de commits acredita que el código evolucionó en el tiempo. No acredita que el estudiante escribió cada línea: es posible hacer commits frecuentes de código generado por IA. Por eso, el repositorio funciona mejor como primera señal que activa otras verificaciones (oral, consignas ancladas) que como evidencia suficiente por sí sola.
