# UniMatch beta.4 · nueva identidad visual

Fecha: **29 de octubre de 2026**. Versión: **0.1.0-beta.4+7**.

## Cambios

- Logo propio: formas entrelazadas que evocan conexión, una U y un corazón.
- Icono Android en cinco densidades, con versión adaptativa y monocromática
  para los iconos temáticos de Android 13 o posterior.
- Logo en acceso, registro, recuperación y confirmación de correo.
- Identidad compartida en el panel administrativo, su favicon, iconos web
  y la página para volver desde el enlace de confirmación de correo.

## Descargar e instalar

Abrir la [Release beta.4](https://github.com/David32361/app_unimach/releases/tag/v0.1.0-beta.4)
y descargar **UniMatch-0.1.0-beta.4.apk** en **Assets**. Instalar sobre la beta.3;
se conserva la firma y se aumenta el código de versión a **7**.

Las betas anteriores y los registros de testers se conservan. Esta actualización
mantiene los cambios de seguridad, verificación por enlace y matches de beta.3.

## Código y diseño

- [PR de implementación #10](https://github.com/David32361/unimach/pull/10).
- [Original, prompt y exportaciones](https://github.com/David32361/unimach/blob/main/branding/README.md).
- [Logo transparente](branding/unimatch-logo.png).
- [Icono sobre fondo claro](branding/unimatch-icon.png).

La publicación sigue siendo una beta. El cambio visual no certifica el recorrido
de verificación con un buzón real y Android que estaba pendiente en beta.3.

## Verificación de la entrega

- APK compilado: `versionName=0.1.0-beta.4`, `versionCode=7`.
- Tamaño: **61 046 195 bytes**.
- SHA-256: `0b933913baa55828e583e56c2ff34d30a49d45de072135c3d27d6dd9d00cfd36`.
- Firma SHA-256: `A1:2A:1F:69:BB:42:5C:DA:E6:32:97:47:F4:58:65:F5:C0:FD:02:15:46:6F:A3:91:21:16:F5:7F:F8:2D:A8:C2`.
- El PNG del logo se comprobó dentro del APK y coincide con el exportado.
- 26 pruebas de usuario y una del panel aprobadas; análisis estático sin incidencias.
- [CI aprobado](https://github.com/David32361/unimach/actions/runs/40887881608).
- Panel web compilado y publicado en Firebase Hosting.
