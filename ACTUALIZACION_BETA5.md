# UniMatch beta.5 · soporte y gestión de cuentas

Versión **0.1.0-beta.5+8**, compilada el 29 de octubre de 2026.

## Disponible en esta APK

- Contacto como texto: **unimatch7@gmail.com**, para quejas, sugerencias y apelaciones.
- Perfil → Eliminar mi cuenta explica cómo solicitar el borrado al soporte desde
  el correo asociado a la cuenta, sin compartir contraseñas. También es accesible
  desde verificación de correo y cuenta sancionada.
- [Instrucciones públicas de eliminación](https://unimatch-daniel-2026.web.app/account-deletion/).
- La moderación registra un aviso privado con el motivo real y el contacto para
  apelar. El panel evita desbordamientos de texto en sus filtros.

## Pendiente de activar

El **borrado automático no está disponible** en esta APK. El proyecto está en Spark,
sin facturación habilitada, y no permite desplegar Cloud Functions. La opción
administrativa de eliminación permanente está deshabilitada; no simula un borrado
marcando únicamente el perfil. Se compiló explícitamente con
`ACCOUNT_MANAGEMENT_ENABLED=false`.

El backend de eliminación propia y administrativa ya está implementado y probado
con datos ficticios. Exige identidad reciente, protege cuentas administrativas,
borra los datos relacionados y reintenta errores. No se borraron cuentas reales.
Véase [estado y activación](GESTION_CUENTAS.md).

Firebase Authentication no permite enviar avisos arbitrarios de baneo o eliminación
con el remitente nativo de verificación. No se envió ningún correo de ese tipo.
Los avisos disponibles son dentro de la app; si el acceso ya fue desactivado,
se muestra el contacto para solicitar revisión.

## Comprobaciones y evidencia

- Análisis de usuario y panel sin incidencias.
- 27 pruebas de usuario y 2 pruebas adicionales del borrado habilitado con dobles.
- 3 pruebas del panel, incluida la protección de la eliminación no disponible.
- 4 pruebas de reglas y 6 de backend en emulador: aislamiento, permisos, reintentos
  y conservación de cuentas y conversaciones ajenas.
- [PR de código #11](https://github.com/David32361/unimach/pull/11).
- [GitHub Actions aprobado](https://github.com/David32361/unimach/actions/runs/40923433572).
- APK release: paquete `com.unimatch.unimatch_user`, versión `0.1.0-beta.5`, código `8`.
- Firma persistente, compatible para actualizar desde beta.4.
- SHA-256 del APK: `f36522ed73c4eab515b7b5f41f573e86e1e4783807c0dec587235a80c2ac1da6`.

[Descargar la beta.5](https://github.com/David32361/app_unimach/releases/tag/v0.1.0-beta.5).
En la Release abre **Assets → UniMatch-0.1.0-beta.5.apk**. Se puede instalar sobre
la beta anterior. El APK de la raíz del repositorio sigue siendo la beta.2 histórica.
