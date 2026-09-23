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

## Desarrollo y releases

- `dev/` contiene builds experimentales que pueden cambiar sin mantener
	compatibilidad entre versiones.
- `release/` contiene builds preparados para su distribución.
