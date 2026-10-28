# Respuesta a testers · beta.3

Entrega de correcciones del **28 de octubre de 2026**, con vencimiento a las
**22:00 America/Mexico_City**. Versión Android: **0.1.0-beta.3+6**.

| Reporte consolidado | Cambio | PR del código |
| --- | --- | --- |
| Contraseñas débiles | 8–128 caracteres, mayúscula, minúscula, número y símbolo; política aplicada en Firebase | [#5](https://github.com/David32361/unimach/pull/5) |
| Uso de correo inventado sin confirmación | Enlace Firebase obligatorio antes de acceder al perfil y a los datos; comprobación al volver a la app | [#5](https://github.com/David32361/unimach/pull/5) |
| Like sin estado claro | Intereses enviados visibles, explicación de reciprocidad y guardado atómico de match/conversación | [#6](https://github.com/David32361/unimach/pull/6) |
| «anos» en perfil | «años» y corrección de acentos en las pantallas | [#7](https://github.com/David32361/unimach/pull/7) |
| «Texnologica» | Corrección del error heredado y normalización de nombres oficiales al mostrar/guardar | [#7](https://github.com/David32361/unimach/pull/7) |

El reporte «no se ven todos los usuarios» se excluyó por indicación del responsable,
quien comprobó que sí aparecen. No se modificaron la consulta ni la paginación
de Descubrir. La edición de perfil fue reportada como correcta y se conserva.

Los reportes originales permanecen en los archivos de [Juan Pablo](juan-pbs/README.md),
[Gael](GaelSilis/README.md) y [Jhoana](Jhoa-ml/README.md). El registro del docente
no contiene hallazgos. La repetición de «años» se consolidó en una sola corrección.

## Pruebas y límites

- Usuario: **26 pruebas aprobadas** y análisis estático sin incidencias.
- Panel: **1 prueba aprobada** y análisis estático sin incidencias.
- Reglas: **3 pruebas aprobadas** en emulador, con cuentas no verificadas,
  reciprocidad del match y protección de participantes.
- Funciones TypeScript: compilación aprobada.
- CI: [PR #8](https://github.com/David32361/unimach/pull/8).

Hace falta comprobar el recorrido completo de correo real y regreso a Android
en un teléfono con esta beta instalada. Si confirmas en otro dispositivo, vuelve
a la app en tu teléfono y pulsa **Ya confirmé mi correo**. El enlace de continuación
no demuestra la confirmación: la app consulta el estado a Firebase.

La beta.2 no incluye esa pantalla y debe actualizarse para usar cuentas cuyo
correo todavía no esté confirmado tras la publicación de las reglas.

## Evidencia del flujo de trabajo

El código sigue ramas por responsabilidad: `feature/seguridad-correo`,
`fix/interacciones-match`, `fix/diseno-ortografia` y `chore/flujo-trabajo`.
La revisión final de lectura transaccional está en `fix/lectura-conversacion`
([PR #9](https://github.com/David32361/unimach/pull/9)).
Cada rama contiene commits y su PR; `main` conserva merges explícitos.
En este repositorio, `docs/resultados-beta3` registra la distribución y la
respuesta a los testers. Las versiones se publican con tags y Releases
preliminares; no se declara estable una beta pendiente de validación en teléfono.

## APK de esta entrega

- Archivo en la Release: `UniMatch-0.1.0-beta.3.apk`.
- Nombre de versión verificado: `0.1.0-beta.3`; código: `6`.
- SHA-256: `fa7f3160ebef950c67f996afe4db5fe1a36ba62fcac1f9ea00b8d37586611296`.
- Firma: misma clave de distribución persistente de beta.2.
- La página de regreso a Android y la asociación del paquete están publicadas
  en Firebase Hosting y responden HTTP 200.
