# Protocolo de coordinación de agentes

## Objetivo

Definir un proceso común para que varios agentes trabajen en el repositorio sin duplicar cambios, perder contexto o aprobar su propio trabajo.

## Roles

- agente de contenido y SEO;
- agente frontend;
- agente de endpoints y datos;
- agente QA;
- agente revisor;
- responsable humano.

## Inicio de una tarea

Antes de modificar archivos, el agente responsable debe:

1. leer `AGENTS.md`;
2. leer `CLAUDE.md` si trabaja con Claude Code;
3. leer `memory.md`;
4. revisar la tarea en `docs/tareas.md`;
5. revisar el estado del repositorio;
6. identificar archivos que probablemente modificar;
7. declarar riesgos y dependencias.

## Flujo recomendado

```text
pendiente
→ en análisis
→ listo para implementación
→ en implementación
→ en revisión
→ cambios solicitados
→ aprobado
```

También existen los estados:

```text
bloqueado
cancelado
```

## Separación de responsabilidades

- Un agente implementa.
- Otro agente revisa.
- La persona responsable aprueba decisiones de contenido, legal, arquitectura, datos y producción.
- El agente que implementa no es el único responsable de aprobar su trabajo.

## Parallel

Solo se ejecutan tareas en paralelo cuando:

- no modifican los mismos archivos;
- no dependen una de otra;
- el responsable humano lo autoriza;
- cada tarea tiene un objetivo independiente.

## Cierre

Toda tarea debe terminar con un handoff que incluya:

- objetivo;
- estado;
- archivos modificados;
- cambios realizados;
- pruebas ejecutadas;
- resultados;
- pendientes;
- riesgos;
- decisiones que requieren aprobación;
- siguiente paso.
