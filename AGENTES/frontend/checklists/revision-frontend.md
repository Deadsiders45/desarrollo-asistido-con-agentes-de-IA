# Checklist de revisión frontend

## Estructura

- [ ] Usa Astro correctamente.
- [ ] Mantiene TypeScript estricto.
- [ ] No introduce `any` sin justificación.
- [ ] No modifica dependencias sin autorización.
- [ ] Usa componentes reutilizables.

## Contenido

- [ ] Los datos provienen de `contenido/`.
- [ ] No hay cifras hardcodeadas.
- [ ] No hay afirmaciones sin soporte.
- [ ] No hay referencias no autorizadas a GPS.
- [ ] No hay logos sin autorización.

## Accesibilidad

- [ ] La página funciona con teclado.
- [ ] El foco es visible.
- [ ] Los encabezados tienen jerarquía correcta.
- [ ] Las imágenes tienen texto alternativo.
- [ ] Los formularios tienen etiquetas.
- [ ] Los errores están asociados a sus campos.

## Rendimiento

- [ ] Las imágenes están optimizadas.
- [ ] Las imágenes tienen dimensiones.
- [ ] No hay JavaScript innecesario.
- [ ] La página funciona bien en móvil.

## Validaciones

- [ ] `npm run check` pasó.
- [ ] `npm test` pasó.
- [ ] `npm run build` pasó.
- [ ] Se documentaron los pendientes.
- [ ] El handoff está completo.
