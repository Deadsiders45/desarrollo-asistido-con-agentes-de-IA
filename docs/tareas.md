# Registro de tareas

## Estados

- `pendiente`
- `en análisis`
- `listo para implementación`
- `en implementación`
- `en revisión`
- `cambios solicitados`
- `aprobado`
- `bloqueado`
- `cancelado`

## Tareas iniciales

| ID | Tarea | Responsable | Estado | Dependencias | Resultado esperado |
|---|---|---|---|---|---|
| SETUP-001 | Configurar `AGENTS.md` | Responsable humano | pendiente | — | Reglas del proyecto completadas |
| SETUP-002 | Configurar `CLAUDE.md` | Responsable humano | pendiente | SETUP-001 | Claude adaptado al proyecto |
| SETUP-003 | Configurar `memory.md` | Responsable humano | pendiente | — | Memoria inicial |
| SETUP-004 | Definir estructura de aplicación | Agente frontend | pendiente | SETUP-001 | Estructura creada |
| SETUP-005 | Definir stack y comandos | Responsable humano | pendiente | SETUP-001 | Stack documentado |
| SETUP-006 | Crear sistema de contenido | Agente de contenido | pendiente | SETUP-001 | Fuente de verdad definida |
| SETUP-007 | Configurar validaciones | Agente QA | pendiente | SETUP-004 | Pruebas ejecutables |
| SETUP-008 | Probar agentes | Responsable humano | pendiente | SETUP-002, SETUP-004 | Primer flujo validado |

## Reglas

- una tarea tiene responsable;
- una tarea no se aprueba sin revisión independiente cuando corresponda;
- las tareas bloqueadas indican la causa;
- no se inician tareas con dependencias pendientes sin autorización;
- cada cambio de estado se registra en el handoff.
