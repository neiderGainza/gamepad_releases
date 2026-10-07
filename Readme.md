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

## Descargas

La página `index.html` sirve los instaladores directamente desde este directorio:

- `linux/` contiene los paquetes `.deb`, `.rpm` y `.pkg.tar.zst`.
- `windows/` contiene `MobileGamePad-Setup.exe`.

Al actualizar un paquete, conserva o actualiza el nombre de archivo y asegúrate
de que la ruta correspondiente en `index.html` coincida. Si la página se publica
como sitio estático, incluye estas carpetas junto a `index.html` para que los
enlaces de descarga funcionen.
