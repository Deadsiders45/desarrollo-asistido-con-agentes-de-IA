# Checklist de revisión de endpoints y datos

## Validación

- [ ] El esquema se comparte entre cliente y servidor.
- [ ] Se validan correos, teléfonos, fechas y límites.
- [ ] Los campos no previstos se rechazan.
- [ ] La fecha de servicio no acepta fechas pasadas cuando corresponda.

## Seguridad

- [ ] Turnstile se verifica en el servidor.
- [ ] Se valida el origen de la petición.
- [ ] Existe rate limiting.
- [ ] Se evita el doble envío.
- [ ] No se exponen secretos.
- [ ] No se imprimen variables de entorno.

## Privacidad

- [ ] No se registran nombres en logs.
- [ ] No se registran correos en logs.
- [ ] No se registran teléfonos en logs.
- [ ] No se registran contenidos de formularios.
- [ ] No se guardan IP en texto claro.
- [ ] No se solicitan documentos innecesarios.

## Persistencia y correo

- [ ] Se registra la versión de la política aceptada.
- [ ] El consentimiento se guarda antes de la solicitud.
- [ ] La solicitud se conserva si falla el correo.
- [ ] Se genera un radicado legible.
- [ ] La migración se puede aplicar desde cero.
- [ ] La eliminación por retención está probada.

## Entrega

- [ ] Las pruebas pasan.
- [ ] Los casos de error están probados.
- [ ] El handoff está completo.
- [ ] Los riesgos están documentados.
