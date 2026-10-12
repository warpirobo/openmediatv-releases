# Arios TV

**Tu biblioteca, tus fuentes, tu televisión.**

[![Android TV](https://img.shields.io/badge/Android_TV-Android_7%2B-3DDC84?logo=android)](https://github.com/warpirobo/openmediatv-releases/releases/latest)
[![Fire TV](https://img.shields.io/badge/Fire_TV-Compatible-FF9900)](https://github.com/warpirobo/openmediatv-releases/releases/latest)
[![Descargar](https://img.shields.io/github/v/release/warpirobo/openmediatv-releases?label=Descargar)](https://github.com/warpirobo/openmediatv-releases/releases/latest)
[![Buy me a coffee](https://img.shields.io/badge/%E2%98%95_Buy_me_a_coffee-PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white)](https://www.paypal.com/paypalme/ITARIOS)

Arios TV es una biblioteca multimedia y reproductor diseñado para el mando de
**Android TV y Fire TV**. Explora tus fuentes rclone, identifica películas y
series, continúa donde ibas y organiza favoritos por perfil. IPTV y TorBox son
opcionales: tú decides cuáles habilitar.

*Remote-first Android TV / Fire TV media library and player for rclone remotes,
with optional IPTV, TorBox, profiles, favorites and automatic updates.*

## Funciones principales

- **rclone integrado:** OneDrive / SharePoint, Google Drive, crypt, combine y otros remotes compatibles. Importación de `rclone.conf` y conexión guiada, sin montar unidades.
- **Biblioteca visual:** películas, series, episodios, colecciones opcionales y versiones de un mismo título. Metadatos y carátulas de TMDB / TheTVDB y otros proveedores compatibles.
- **Reproducción:** Media3 / ExoPlayer, ASS con libass, estilo Custom OpenHub y selección de pistas. FFmpeg ofrece decodificación alternativa de audio cuando corresponde; la compatibilidad final depende del archivo, dispositivo y equipo de audio.
- **Perfiles:** historial, progreso y favoritos separados, opciones para menores y PIN opcional.
- **IPTV opcional:** listas remotas TXT / M3U, búsqueda, favoritos y varias fuentes para un mismo canal.
- **TorBox opcional:** películas, series, anime, Mis torrents, favoritos, continuar viendo y filtros de idiomas, resolución y edición. Temporadas y episodios con imágenes cuando el proveedor las ofrece.
- **Proveedores externos:** Torrentio, Comet, Hydra, MediaFusion y addons configurables. DeepFlix y PlavioHD ofrecen enlaces HTTPS directos, fuera de la caché TorBox. No se comparte la clave TorBox con esos addons.
- **Subtítulos online:** OpenSubtitles y Subtitulamos.tv para series, desde el reproductor TorBox. Disponibilidad y sincronización dependen del proveedor y la versión del vídeo.
- **Trackers:** conexión opcional con SIMKL y WeTrakr.
- **Mantenimiento:** backups seleccionables, diagnóstico de reproducción y actualizaciones desde la aplicación.

## Descargar e instalar

1. Abre [el último release](https://github.com/warpirobo/openmediatv-releases/releases/latest).
2. Descarga la APK **public-armeabi-v7a-release.apk** para televisión.
3. Permite la instalación desde la herramienta de descarga y confirma en Android.
4. Elige idioma y fuentes. Activa los servicios opcionales en **Ajustes → IPTV · TorBox**.

Requisito mínimo: **Android 7 / API 24**. Este canal distribuye la variante TV,
no la versión móvil con Cast. Algunas funciones dependen del fabricante.

## Actualizar sin perder la configuración

Ve a **Ajustes → Actualizaciones de la aplicación**. Descarga y confirma la
instalación cuando Android lo solicite. Tras instalar correctamente, la app limpia
el instalador que ella descargó; no borra APK guardadas manualmente en otras carpetas.

**Actualiza sin desinstalar.** Conserva preferencias, cuentas y claves previamente
guardadas. Los datos de la antigua variante TorBox separada no se migran
automáticamente a la aplicación normal.

## Claves y privacidad

La APK pública **no incluye claves privadas de TMDB / TheTVDB**. En instalaciones
nuevas, introduce las tuyas desde los ajustes de proveedores. Las versiones puente
guardan las existentes localmente para conservarlas al actualizar. Las credenciales
se cifran en el dispositivo y no se publican aquí.

El código de Arios TV permanece privado. Este repositorio contiene descargas,
notas y `update.json`, no configuraciones personales ni claves de firma. Los
servicios opcionales se comunican con sus respectivos proveedores. Arios TV
no proporciona contenido precargado ni cuentas de terceros.

## Límites y disponibilidad

- Calidad e idioma usan las etiquetas declaradas en las fuentes; una carátula no garantiza una versión 4K disponible.
- Mis torrents indexa progresivamente hasta 10.000 resúmenes por cuenta, con aviso del límite. El primer recorrido puede tardar; las visitas siguientes usan el índice local.
- Aquí no se importan los catálogos deportivos en vivo de PlavioHD.
- Las webs de FMHY no son todas addons compatibles ni se convierten automáticamente en proveedores.
- Las capacidades de audio/vídeo y la disponibilidad de servicios dependen del dispositivo y proveedor. Consulta el alcance de verificación en cada release.

## Ayuda y diagnósticos

[Abre una incidencia](https://github.com/warpirobo/openmediatv-releases/issues)
con modelo de dispositivo, versión de Arios TV y pasos del problema. Revisa el
diagnóstico antes de compartirlo: **no publiques contraseñas, tokens, claves,
configuraciones rclone ni enlaces privados**.

## Componentes y licencias

AndroidX Media3, FFmpeg, libass, rclone y sus dependencias. Consulta **Acerca de →
Licencias** dentro de la app. Los releases adjuntan las fuentes correspondientes
de FFmpeg y recetas de compilación. Los proveedores son independientes; sus
condiciones, disponibilidad y derechos de contenido no los controla Arios TV.

## Apoya el proyecto

[☕ Invítame a un café por PayPal](https://www.paypal.com/paypalme/ITARIOS)

El mismo enlace de apoyo de [rclone-nexus-kodi](https://github.com/warpirobo/rclone-nexus-kodi).
