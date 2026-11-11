# Gestión del proyecto en monday.com

El seguimiento ágil de PAEGo (Metodología de Software Colaborativo) vive en el
espacio de trabajo **PAEGo** de monday.com, del 10 de agosto al 16 de noviembre de 2026.

| Tablero | Para qué sirve |
|---|---|
| 1. Backlog | Historias de usuario con prioridad, puntos y requisito (RF/RNF) |
| 2. Sprints y tareas | Tareas por sprint (7 sprints de dos semanas + entrega final) |
| 3. Sprints | Objetivo, fechas, velocidad y retrospectiva de cada sprint |
| 4. QA | Casos de prueba por suite y su resultado |

El tablero de control reúne puntos, horas, avance del backlog, el Gantt y los
resultados de pruebas.

## Integración con GitHub

`.github/workflows/monday.yml` refleja cada pull request en "2. Sprints y tareas":

| Evento del PR | Estado en monday |
|---|---|
| Borrador | En curso |
| Abierto o listo para revisión | En revisión |
| Fusionado | Hecho |
| Cerrado sin fusionar | Pendiente |

El elemento cae en el grupo del sprint según la fecha del PR, con responsable,
tipo, cronograma y enlace, y cada evento deja un comentario. Usa la API de monday
con el secreto `MONDAY_TOKEN`.
