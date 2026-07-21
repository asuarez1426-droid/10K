# Plantilla — CRM de prospectos en Notion

Crea una **base de datos** en Notion llamada `CRM — Operación 10K` con esta estructura exacta. (Si me confirmas en el chat, la creo yo directamente en tu Notion.)

## Propiedades (columnas)

| Propiedad | Tipo en Notion | Valores / detalle |
|---|---|---|
| Nombre | Título | Nombre completo del prospecto |
| Estado | Select | `Nuevo` `Contactado` `Respondió` `Llamada agendada` `Llamada hecha` `Propuesta enviada` `🏆 CLIENTE` `Perdido` `No calificado` |
| Nicho | Select | `Coaches/consultores` `Dueños de negocio` `Profesionales alto valor` (ajusta al cerrar el sprint) |
| Canal | Select | `LinkedIn` `Instagram` `Referido` `Entrante (contenido)` |
| Link perfil | URL | Perfil de LinkedIn o IG |
| Observación personal | Texto | La nota que personaliza el primer mensaje (obligatoria antes de contactar) |
| Fecha primer contacto | Fecha | |
| Último toque | Fecha | Se actualiza en cada interacción |
| Próxima acción | Fecha | Motor de los seguimientos: día 3, 7, 14, 30 |
| Nº de toques | Número | Máximo 5, luego `Perdido` |
| Valor potencial | Select | `Retainer 3.5M` `Consultoría 1.5M` `Auditoría 800K` |
| Notas | Texto | Qué dijo, objeciones, contexto |

## Vistas a crear

1. **📥 Pipeline** — Tablero (board) agrupado por `Estado`. Tu vista principal: los prospectos se arrastran de columna en columna.
2. **🔥 Toques de hoy** — Tabla filtrada: `Próxima acción` es hoy o antes, y `Estado` no es `CLIENTE`/`Perdido`/`No calificado`. Ordenada por `Próxima acción`. **Esta vista ES tu bloque de seguimientos diario.**
3. **📞 Llamadas** — Tabla filtrada: `Estado` = `Llamada agendada` o `Llamada hecha`.
4. **🏆 Clientes** — Tabla filtrada: `Estado` = `CLIENTE`.
5. **📊 Por nicho** — Tablero agrupado por `Nicho` (para el sprint de validación de la semana 1).

## Reglas de uso

- Ningún prospecto entra sin `Observación personal` y `Link perfil`.
- Cada interacción actualiza `Último toque`, `Nº de toques` y `Próxima acción`. 15 min al final del Bloque 1, todos los días.
- Domingo: cuenta los totales por estado para el scorecard (doc 09).

## Página complementaria: `Dashboard — Operación 10K`

Página simple encima del CRM con: la tabla de hitos del README, el scorecard de la semana en curso (doc 09) y los enlaces a los guiones. Es tu página de inicio de cada mañana.
