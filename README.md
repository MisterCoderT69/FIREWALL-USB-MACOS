FIREWALL-USB-MACOS

Un proyecto para macOS que permite bloquear temporalmente dispositivos USB, como memorias y periféricos, protegiendo el sistema y controlando el acceso a los puertos de manera segura y configurable.

⚔️ Características

Bloqueo temporal de todos los dispositivos USB o selectivos (memorias, mouse, etc.).

Control en tiempo real de la conexión de USB.

Compatible con macOS y optimizado para trabajar con la arquitectura moderna de Apple.

Uso de IOKit para la detección y manejo de dispositivos USB.

Configuración de tiempos de bloqueo automáticos.

⚔️ Requisitos

macOS 10.15 o superior

Python 3.x

Permisos de administrador (sudo)

Xcode Command Line Tools (opcional para extensiones avanzadas)

⚔️ Instalación

Clonar el repositorio:

git clone https://github.com/tuusuario/FIREWALL-USB-MACOS.git
cd FIREWALL-USB-MACOS


Ejecutar el script principal:

sudo python3 firewall_usb.py

⚔️ Uso

El script detecta dispositivos USB conectados.

Permite decidir si se permite o bloquea cada dispositivo.

Se puede configurar un tiempo de bloqueo automático, por ejemplo 30 segundos.

Posibilidad de aplicar filtros para bloquear solo:

Memorias externas

Mouse USB

Otros dispositivos HID sin afectar periféricos críticos

⚔️ Integración con IOKit

FIREWALL-USB-MACOS utiliza IOKit para:

Detectar dispositivos USB conectados en tiempo real.

Obtener información de cada dispositivo (tipo, VendorID, ProductID).

Permitir o bloquear dispositivos dinámicamente sin comprometer la estabilidad del sistema.

⚔️ Advertencias

⚠️ Precaución:

Bloquear todos los puertos USB puede desactivar teclados y mouse externos.

Siempre tener un teclado interno o Bluetooth activo antes de usar.

No está diseñado para entornos críticos donde la pérdida de control del sistema pueda causar problemas.

⚔️ Contribuciones

Se aceptan contribuciones para:

Mejorar la detección de dispositivos HID

Crear interfaces gráficas amigables

Soporte para tiempos de bloqueo personalizados y reglas avanzadas

⚔️ Licencia

Este proyecto está bajo la licencia MIT.
