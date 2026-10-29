# UniMatch · distribución y resultados de pruebas

<img src="branding/unimatch-icon.png" width="160" alt="Logo de UniMatch">

## Actualización beta.5 · 29 de octubre de 2026

- Versión: **0.1.0-beta.5+8**.
- [Descargar APK beta.5](https://github.com/David32361/app_unimach/releases/tag/v0.1.0-beta.5).
- Contacto para quejas, sugerencias y apelaciones: **unimatch7@gmail.com**.
- Perfil → Eliminar mi cuenta muestra cómo solicitar el borrado al soporte.
- [Instrucciones fuera de la app](https://unimatch-daniel-2026.web.app/account-deletion/).
- Los avisos privados de sanción incluyen motivo y opción de apelar.
- **El borrado automático aún no está activo**: el proyecto Firebase usa Spark.
  La opción administrativa permanente permanece deshabilitada hasta activar el backend.
- No se envían correos personalizados de baneo o eliminación con el remitente
  de verificación de Firebase: ese servicio no permite mensajes arbitrarios.
- [Disponibilidad y requisitos de activación](GESTION_CUENTAS.md).
- [Notas y comprobaciones](ACTUALIZACION_BETA5.md).
- Mantiene la firma de la beta.4; se puede instalar sobre la versión anterior.

## Actualización beta.4 · 29 de octubre de 2026

- Versión: **0.1.0-beta.4+7**, con el nuevo logo de UniMatch.
- [Descargar APK beta.4](https://github.com/David32361/app_unimach/releases/tag/v0.1.0-beta.4).
- Icono Android normal, adaptativo y temático; logo en acceso, registro,
  recuperación, confirmación de correo y panel administrativo.
- Instalar sobre la beta.3: conserva la misma firma y aumenta el código de versión.
- El original transparente está en [branding/unimatch-logo.png](branding/unimatch-logo.png).
- [Notas y verificación de la actualización](ACTUALIZACION_BETA4.md).

## Actualización beta.3 · 28 de octubre de 2026

- Versión: **0.1.0-beta.3+6**.
- [Descargar la beta.3 anterior en GitHub Releases](https://github.com/David32361/app_unimach/releases/tag/v0.1.0-beta.3).
- [Correcciones y comprobaciones](RESULTADOS_BETA3.md).
- [Ramas, PRs y flujo de trabajo del código](https://github.com/David32361/unimach/blob/main/docs/FLUJO_GITHUB.md).

Esta actualización requiere confirmar el correo mediante el enlace de Firebase.
Abre el correo, confirma y pulsa **Continuar** para volver a la app. Si no se abre,
pulsa **Abrir UniMatch** o vuelve a la app y selecciona **Ya confirmé mi correo**.
Las cuentas con Google cuyo correo ya está verificado continúan normalmente.

Los apartados siguientes conservan las instrucciones y resultados de la ronda
**beta.2**, cerrada el 25 de octubre. El APK de la raíz es la beta.2 histórica;
la versión actual se descarga desde la Release beta.5, sin reemplazar las anteriores.

## Periodo y participantes

- **Fecha limite para registrar hallazgos:** 25 de octubre de 2026 a las 23:59, hora de Ciudad de Mexico.
- **Participantes:** [Juan Pablo (`juan-pbs`)](juan-pbs/README.md), [Gael (`GaelSilis`)](GaelSilis/README.md), [Jhoana (`Jhoa-ml`)](Jhoa-ml/README.md) y [docente (`DSRG80`)](DSRG80/README.md).
- **Version a revisar:** UniMatch 0.1.0-beta.2, build 5.
- **Descarga del APK:** abre la [Release 0.1.0-beta.2](https://github.com/David32361/app_unimach/releases/tag/v0.1.0-beta.2) y descarga `UniMatch-0.1.0-beta.2.apk` en **Assets**. El mismo archivo tambien esta en la raiz de este repositorio.

Instala el APK en un dispositivo Android 7.0 o posterior. Si Android lo solicita,
autoriza la instalacion desde la aplicacion con la que descargaste el archivo.
Si ya tienes la beta anterior firmada, instala esta version sobre ella.

SHA-256 del APK:
`2a85a878103fb2ab3a6e743ac1ce817856a7091e049ff698eee9050c47bb40ff`

## Como registrar un hallazgo

Cada participante escribe sus resultados en su propio README, en la rama `main`:

- [Tabla de Juan Pablo](juan-pbs/README.md)
- [Tabla de Gael](GaelSilis/README.md)
- [Tabla de Jhoana](Jhoa-ml/README.md)
- [Tabla del docente](DSRG80/README.md)

Por cada hallazgo, anota fecha, dispositivo y version de Android. En
**Hallazgo**, explica los pasos, lo que esperabas y lo que sucedio. En
**Estado**, escribe `Reportado`. Solo edita tu propio archivo para evitar
conflictos con los registros de los demas.

No es obligatorio crear un issue. Si lo haces, agrega el enlace en la columna
**Issue (opcional)**; si no, deja `-`. El [issue general de pruebas](https://github.com/David32361/app_unimach/issues/1)
tambien permanece abierto para preguntas. No publiques contrasenas, correos,
codigos de acceso ni capturas con datos personales.

## Cierre y privacidad

La ronda recibe comentarios hasta el **25 de octubre de 2026 a las 23:59**,
hora de Ciudad de Mexico. A partir del 26 de octubre no agregues hallazgos
nuevos; los registros y el APK seguiran disponibles para consulta.

Consulta la [politica de privacidad](PRIVACIDAD.md). Esta beta no esta
aprobada para Amazon Appstore. Este repositorio distribuye la app y registros
de prueba; no contiene el codigo fuente.
