# AGENTS.md

## Propósito

Este archivo es la fuente común de instrucciones para los agentes de IA que trabajan en este proyecto.

Cada agente debe leer este archivo antes de modificar archivos.

También debe leer, cuando corresponda:

- `memory.md` — memoria del proyecto y errores corregidos;
- `docs/tareas.md` — registro de tareas;
- `docs/handoff.md` — formato de entrega;
- `docs/orquestacion.md` — protocolo de coordinación;
- `docs/politica-skills.md` — política de skills;
- la documentación específica del proyecto.

## Configuración del proyecto

Antes de trabajar, el agente debe identificar y documentar:

- nombre del proyecto;
- objetivo;
- alcance permitido;
- funcionalidades excluidas;
- stack aprobado;
- estructura de carpetas;
- comandos disponibles;
- variables de entorno requeridas, sin exponer valores;
- datos confirmados;
- datos pendientes;
- datos conflictivos;
- decisiones que requieren autorización humana.

No se debe asumir que la configuración de este archivo corresponde a un proyecto específico hasta que sea completada.

## Alcance

El agente debe trabajar únicamente dentro del alcance aprobado.

No debe agregar funcionalidades, proveedores, integraciones o cambios arquitectónicos sin autorización expresa.

## Arquitectura

El agente debe respetar el stack aprobado por el proyecto.

Si necesita una tecnología no aprobada, debe detenerse, explicar qué necesita, indicar riesgos y alternativas, y solicitar aprobación.

## Fuente de verdad

El proyecto debe definir explícitamente dónde viven los datos de negocio.

Regla general:

> Todo dato de negocio, texto corporativo, cifra, teléfono, correo, dirección o afirmación pública debe provenir del archivo o sistema de contenido aprobado.

El agente no debe escribir información de negocio directamente en páginas, componentes o lógica de presentación.

## Datos

El agente debe diferenciar:

- confirmado;
- pendiente;
- conflictivo;
- no autorizado;
- sin soporte;
- oculto temporalmente.

No debe inventar, deducir ni publicar datos no confirmados.

## Seguridad y privacidad

- no exponer secretos;
- no imprimir variables de entorno;
- no copiar claves a archivos;
- no hacer commits con `.env`;
- no registrar datos personales en logs;
- no deshabilitar validaciones de seguridad;
- no modificar producción sin autorización;
- no ejecutar migraciones destructivas sin confirmación;
- no eliminar datos sin confirmación;
- no realizar despliegues sin autorización.

## Skills

Las skills disponibles se encuentran en la carpeta de skills del agente correspondiente.

La fuente principal de skills del proyecto es:

```text
.agents/skills/
```

Claude Code utiliza normalmente:

```text
.claude/skills/
```

Las skills son guías operativas. No reemplazan las reglas de este archivo ni autorizan cambios fuera del alcance.

## Roles

Los roles disponibles son:

- contenido y SEO;
- frontend;
- endpoints y datos;
- QA;
- revisor;
- coordinador;
- responsable humano.

El agente que implementa no debe ser el único responsable de aprobar su propio trabajo.

## Flujo de trabajo

1. leer `AGENTS.md`;
2. leer `memory.md` y la documentación relevante;
3. revisar el estado del repositorio;
4. revisar `docs/tareas.md`;
5. identificar objetivo, archivos y riesgos;
6. proponer plan para tareas no triviales;
7. esperar aprobación cuando corresponda;
8. implementar;
9. ejecutar validaciones;
10. revisar los cambios;
11. completar el handoff;
12. reportar resultados, riesgos y pendientes.

## Validaciones

Según corresponda, el agente debe ejecutar:

- comprobación de tipos;
- linting;
- pruebas unitarias;
- pruebas de integración;
- build;
- pruebas end-to-end;
- revisión de accesibilidad;
- revisión de enlaces;
- revisión de rendimiento;
- revisión de contenido;
- revisión de seguridad;
- revisión de formularios.

## Criterios de finalización

Una tarea no puede marcarse como completada si:

- falla el build;
- fallan pruebas relevantes;
- existen errores de tipos;
- existen errores relevantes de lint;
- queda una decisión pendiente;
- se introdujeron afirmaciones sin soporte;
- se modificaron datos no autorizados;
- se expusieron secretos;
- quedaron riesgos de seguridad o privacidad sin resolver.

## Reporte obligatorio

Todo agente debe cerrar su tarea con:

- objetivo;
- archivos modificados;
- cambios realizados;
- pruebas ejecutadas;
- resultados;
- pendientes;
- riesgos;
- decisiones que requieren aprobación;
- siguiente paso recomendado.

## Configuración inicial pendiente

Antes de usar este sistema en un proyecto nuevo, se deben reemplazar o completar las referencias específicas del proyecto en:

- `AGENTS.md`;
- `CLAUDE.md`;
- `memory.md`;
- `docs/tareas.md`;
- `docs/orquestacion.md`;
- `AGENTES/`.

No se debe comenzar a implementar antes de completar esa configuración.
