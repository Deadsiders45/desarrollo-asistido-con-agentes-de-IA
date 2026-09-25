# Política de skills y ubicaciones

## Fuente principal

La ubicación principal de las skills instaladas es:

```text
.agents/skills/
```

Esta carpeta contiene las skills universales del proyecto.

## Claude Code

Claude Code utiliza:

```text
.claude/skills/
```

- las carpetas pueden ser enlaces hacia `.agents/skills/`;
- si el instalador crea una copia, debe considered compatible solo si tiene el mismo contenido;
- Claude debe verificar la skill antes de usarla.

## Otros agentes

La carpeta:

```text
agent/skills/
```

se conserva como ubicación de compatibilidad para agentes que utilizan esa convención.

No se debe modificar manualmente una skill para resolver un problema de un solo agente. Los cambios se realizan en la fuente principal y luego se verifica la sincronización.

## Reglas

- no eliminar skills sin autorización;
- no instalar skills sin autorización;
- no mezclar versiones de una misma skill;
- registrar la instalación en `skills-lock.json`;
- revisar el contenido de una skill antes de usarla;
- no aplicar automáticamente patrones de otro framework o proveedor;
- `review-and-refactor` requiere revisión manual y pruebas.
