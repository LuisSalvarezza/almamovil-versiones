# Alma Móvil — versiones publicadas

Desde la versión 4.16 la app lee el aviso de versión nueva de
`https://luissalvarezza.github.io/almamovil-versiones/app/version.json` y baja el APK de la Release
que indica ese archivo (lo instala desde la pantalla "Actualizar").

- `app/version.json`: última versión publicada (versionCode, versionName, url del APK, sha256,
  novedades y minimaVersionCode).
- Releases `vX.YY`: el APK firmado con el certificado de producción (`AlmaMovil-X.YY.apk`).

Se publica con `tools/PublicarVersion.ps1` del proyecto, con la cuenta LuisSalvarezza.
Los teléfonos con la 4.15 o anteriores leen la dirección vieja (almamovil.github.io): la 4.16 se
les instala una vez a mano.
