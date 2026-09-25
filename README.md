# Sistema general de desarrollo asistido con IA

Este directorio es una plantilla reutilizable del sistema de desarrollo asistido con agentes.

## Propósito

Permite iniciar un nuevo proyecto web y configurar sus reglas para que varios agentes trabajen de forma coordinada.

## Estructura

```text
.agents/       skills principales
.claude/       adaptador para Claude Code
agent/         adaptador para otros agentes
AGENTES/       definiciones de agentes
docs/          coordinación, tareas, handoff y política de skills
AGENTS.md      reglas comunes
CLAUDE.md      reglas específicas para Claude Code
memory.md      memoria y correcciones
agent.md       plantilla histórica
skills-lock.json registro de skills
```

## Configuración para un nuevo proyecto

1. Copiar esta carpeta al proyecto correspondiente.
2. Completar `AGENTS.md`.
3. Completar `CLAUDE.md`.
4. Completar `memory.md`.
5. Crear la estructura de aplicación del proyecto.
6. Crear el archivo de contenido del proyecto.
7. Crear `docs/tareas.md` con las tareas iniciales.
8. Revisar los agentes en `AGENTES/` y ajustar sus permisos.
9. Verificar las skills disponibles.
10. Ejecutar el flujo de prueba de agentes antes de iniciar producción.

## Principios

- la configuración específica vive en los archivos del proyecto;
- las skills son reutilizables;
- los agentes son guías operativas;
- el humano mantiene la autoridad final;
- ninguna tarea se cierra sin pruebas y revisión.
