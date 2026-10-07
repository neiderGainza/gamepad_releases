# Builds

Este directorio contiene los paquetes distribuibles de **Mobile GamePad**.

Mobile GamePad convierte un teléfono móvil en un gamepad para el ordenador. La
aplicación móvil se comunica con un servidor que recibe los eventos de entrada
y permite crear y utilizar dispositivos virtuales mediante `uinput` en Linux.

## Requisitos del servidor

- Linux con soporte para `uinput`.
- Permisos para crear y utilizar dispositivos de entrada virtuales.
- Un archivo `.tar.gz` compatible con la arquitectura del sistema.
- La aplicación móvil Mobile GamePad configurada para conectarse al servidor.

## Publicar una versión

Los instaladores y paquetes se distribuyen como **assets de GitHub Releases**;
el sitio de descargas enlaza directamente a los archivos de la última release.
Así no es necesario servir los binarios desde el repositorio del sitio.

1. Genera los paquetes de la versión y crea una etiqueta, por ejemplo `v0.0.1`.
2. En GitHub, abre **Releases → Draft a new release**, selecciona esa etiqueta y
	adjunta los instaladores/paquetes en **Attach binaries**.
3. Antes de adjuntarlos, usa estos nombres estables para los assets (no incluyas
	la versión en los nombres Linux):
	- `mobile-gamepad-linux-amd64.deb`
	- `mobile-gamepad-linux-x86_64.rpm`
	- `mobile-gamepad-linux-x86_64.pkg.tar.zst`
	- `MobileGamePad-Setup.exe`
4. Publica la release. Puedes renombrar los archivos generados antes de
	adjuntarlos; conserva los nombres anteriores en cada nueva versión.

Los enlaces usan el formato
`https://github.com/neiderGainza/mobile_gamepad/releases/latest/download/NOMBRE_DEL_ARCHIVO`.
Al conservar esos nombres, los enlaces de `index.html` seguirán funcionando sin
cambios en cada nueva versión.

Los builds experimentales no destinados al público pueden mantenerse aparte de
las releases estables.
