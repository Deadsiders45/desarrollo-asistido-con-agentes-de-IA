# CLAUDE.md

## Adapter for Claude Code

La fuente canónica de instrucciones es:

```text
AGENTS.md
```

Claude debe leer `AGENTS.md` antes de trabajar.

También debe leer, cuando corresponda:

- `memory.md`;
- `docs/tareas.md`;
- `docs/handoff.md`;
- `docs/orquestacion.md`;
- `docs/politica-skills.md`;
- `.claude/skills/`;
- la documentación específica del proyecto.

## Reglas mínimas

- no inventar datos;
- no publicar afirmaciones sin soporte;
- no modificar la arquitectura sin autorización;
- no exponer secretos;
- no registrar datos personales en logs;
- no modificar producción sin autorización;
- ejecutar las pruebas correspondientes;
- completar el handoff;
- detenerse cuando falte una decisión.

## Skills

Las skills disponibles para Claude están en:

```text
.claude/skills/
```

Las skills son guías operativas y no reemplazan `AGENTS.md`.

## Flujo mínimo

1. leer `AGENTS.md`;
2. leer `memory.md` y la documentación;
3. revisar el estado del repositorio;
4. identificar objetivo, archivos y riesgos;
5. proponer plan cuando corresponda;
6. esperar aprobación si es necesaria;
7. implementar;
8. validar;
9. revisar;
10. entregar handoff y reporte.

No se debe inventar una respuesta para completar una tarea.
