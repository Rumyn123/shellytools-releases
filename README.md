# ShellyTools — descargas

Repositorio público de instaladores y actualizaciones. El código fuente se mantiene privado. No se almacenan configuraciones, licencias activadas, claves, correos ni datos de clientes aquí.

## Canal de prueba · primera computadora

Las versiones `5.3.0-rc.151` y `5.3.0-rc.152` permiten probar la instalación inicial y luego la actualización desde la aplicación. Consulta [las publicaciones](https://github.com/Rumyn123/shellytools-releases/releases) para verificar su disponibilidad.

1. Guarda y cierra ShellyTools. Conserva tu carpeta anterior; no borres datos ni borradores de Outlook.
2. Descarga `Initialize-UpdateBridge.ps1` de la publicación. Ejecuta el script en PowerShell con `-PreviousDirectory "CARPETA_DE_TU_VERSION_ANTERIOR"`. Copia únicamente la configuración local, sin subirla a Internet.
3. Ejecuta `ShellyTools-test-Setup.exe` de rc151 para probar el salto a rc152. Después usa el acceso directo instalado. En el siguiente inicio la app ofrecerá descargar y, con otra confirmación, actualizar y reiniciar.

Para una instalación directa, usa el instalador de rc152. Las instalaciones antiguas en ZIP no pueden actualizarse hasta completar este puente una sola vez. rc150 fue una construcción local, no una descarga pública.

**Prueba, no producción validada.** Los ejecutables todavía no tienen certificado Authenticode de editor confiable. La firma P-256 del manifiesto y SHA256 verifican las actualizaciones dentro de la app, pero no sustituyen la reputación de SmartScreen. No desactives antivirus ni instales certificados desconocidos. Segunda computadora sólo después de validar la primera.

La app comprueba al iniciar; durante una sesión permite comprobar/descargar, pero instalar requiere guardar, cerrar y abrir. Actualizar nunca envía correos. Sin Internet puedes seguir usando la versión instalada.

Software propietario de Haim Seguros. Los paquetes incluyen avisos y licencias de componentes de terceros. No se otorga una licencia pública del código fuente ni de los assets.
