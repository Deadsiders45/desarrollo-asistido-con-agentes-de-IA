# Checklist de revisión final

## Alcance

- [ ] El objetivo está claro.
- [ ] Los archivos modificados son relevantes.
- [ ] El cambio está dentro del MVP.
- [ ] No se modificaron decisiones arquitectónicas sin autorización.

## Contenido

- [ ] Los datos provienen de `contenido/`.
- [ ] No hay cifras inventadas.
- [ ] No hay afirmaciones sin soporte.
- [ ] Los conflictos están documentados.
- [ ] No hay referencias no autorizadas a GPS.
- [ ] No hay logos sin autorización.
- [ ] Los datos simulados están identificados.

## Técnica

- [ ] `npm run check` pasó.
- [ ] `npm test` pasó.
- [ ] `npm run build` pasó.
- [ ] Las pruebas relevantes están documentadas.
- [ ] No se eliminaron validaciones.
- [ ] Los contratos compartidos se respetan.

## Seguridad y privacidad

- [ ] No hay secretos expuestos.
- [ ] No hay datos personales en logs.
- [ ] No se registran IP en texto claro.
- [ ] Turnstile se verifica en el servidor cuando aplica.
- [ ] Existe rate limiting cuando aplica.
- [ ] La versión de la política se registra.

## Revisión

- [ ] La revisión fue realizada por alguien distinto del implementador.
- [ ] Las observaciones están documentadas.
- [ ] La decisión está registrada.
- [ ] Los pendientes tienen responsable.
- [ ] Las decisiones humanas están identificadas.

## Decisión

- [ ] Aprobado.
- [ ] Cambios solicitados.
- [ ] Rechazado.
- [ ] Aprobado con pendientes.
