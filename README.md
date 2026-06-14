# 🎮 Convertidor Pro

[![GitHub Release](https://img.shields.io/github/v/release/TU_USUARIO/RedumpScraper?label=Versi%C3%B3n&color=blue)](https://github.com/TU_USUARIO/RedumpScraper/releases)
[![Platform](https://img.shields.io/badge/Plataforma-Windows-blueviolet)]

**Convertidor Pro** (desarrollado bajo el ecosistema *RedumpScraper*) es la herramienta definitiva de automatización, conversión y optimización de copias de seguridad de videojuegos. Diseñada tanto para entusiastas de la emulación como para usuarios de hardware real, esta suite unifica los procesos más complejos de descifrado, compresión y cambio de formatos en una interfaz fluida, rápida y automatizada.

¿Tienes carpetas llenas de ISOs que devoran tu disco duro o archivos corruptos que los emuladores rechazan? **Convertidor Pro lo soluciona todo.**

---

## 🚀 Características Principales por Sistema

| Sistema | Formatos de Entrada | Formatos de Salida / Operación | Objetivo / Optimización |
| :--- | :--- | :--- | :--- |
| **🕹️ PlayStation 1** | `.cue` / `.bin` (Múltiples pistas) | `.chd` | **Súper Normalización:** Repara automáticamente archivos `.cue` defectuosos (rutas absolutas, errores de sintaxis en `MODE2` o índices de tiempo) antes de enviarlos a `chdman`. |
| **🚙 PlayStation 2** | `.iso` | `.chd`, `.zso` | Compresión ideal para PCSX2 y formato `.zso` optimizado para carga desde **OPL (Open PS2 Loader)**. |
| **🎮 PSP** | `.iso` | `.chd`, `.zso`, `.cso` | Flexibilidad total de compresión para PPSSPP y hardware real. |
| **💿 PlayStation 3** | `.iso` (Redump encriptado) | ISO descifrada, Formato Carpeta (`JB Folder`) | Descifra imágenes Redump nativas para hacerlas jugables en **RPCS3** o prepararlas en carpetas para tu **PS3 con CFW/HEN**. |
| **🟢 Xbox Clásica** | Formato Carpeta, `.iso` (Redump) | `.xiso` (ISO optimizada), ISO descifrada | Convierte carpetas sueltas a `.xiso` compatible y descifra ISOs complejas de Redump para jugarlas directamente en **Xemu**. |
| **⚪ Xbox 360** | `.iso` | Carpeta `.XEX`, GoD (Games on Demand), `.zar`, `.iso` | Extrae a formato nativo, genera paquetes GoD para consolas con RGH/JTAG, y comprime al formato extremo **`.zar` para el emulador Xenia**. |
| **🌀 Wii & GameCube** | `.iso`, `.gcm`, `.wbfs`, `.rvz` | `.wbfs`, `.rvz`, `.iso` (Scrubbed), `.gcm` | Optimización mediante *Scrubbing* (eliminación de datos basura), conversión a `.wbfs` para loaders de Wii, y compresión `.rvz` sin pérdidas para **Dolphin**. |
| **📐 Nintendo 3DS** | `.cia`, `.3ds`, `.cci` (Redump) | `.3ds`, `.cia`, `.3dsx`, `.cci` descifrado | Intercambio bidireccional entre CIA/3DS, descifrado automático de copias Redump (`.cci`) y conversión a `.3dsx` para el emulador **Azahar**. |
| **🔴 Nintendo Switch**| `.nsp`, `.nsz` | `.nsz`, `.nsp` | Conversión bidireccional de alta velocidad para optimizar almacenamiento en emuladores como Ryujinx/Yuzu. |

---

## 🛠️ ¿Qué hace especial a Convertidor Pro?

* **Smart Bypass de Errores:** Olvídate de los cierres inesperados de las herramientas de consola. Si un `.cue` de PS1 viene mal estructurado desde internet, el software analiza su sintaxis en tiempo real, lo reescribe con el formato correcto y reanuda la conversión a `.chd` de manera invisible para el usuario.
* **Procesamiento Asíncrono en Segundo Plano:** Diseñado sobre tareas asíncronas (`Task.Run`) para asegurar que la interfaz gráfica nunca se congele, reportando el progreso exacto (`%`) de herramientas externas en tiempo real.
* **Automatización "Zero-Config":** El programa incluye e integra de forma interna los binarios y librerías necesarias para que no tengas que pelear con variables de entorno o líneas de comandos tediosas.

---

## 📸 Capturas de Pantalla

![Alt-payload](https://i.imgur.com/Kwmqjkr.png)


---

## 📦 Instalación y Requisitos
Descarga la última versión estable desde la sección de Releases.

Extrae el archivo .zip en una carpeta de tu preferencia.

Ejecuta ConvertidorPro.exe (asegúrate de otorgar permisos de lectura/escritura si trabajas en discos externos).

Requisitos del sistema:

Windows 10 / 11 (64-bit).

.NET Runtime compatible (según la versión de tu compilación).

## 🤝 Contribuciones y Soporte
Si encuentras algún formato rebelde que se resista a la conversión, o si un archivo .cue muy específico logra romper la lógica de súper normalización, por favor abre un Issue adjuntando el log del error o el texto del archivo afectado. ¡Toda ayuda para pulir la herramienta es bienvenida!

## 📄 Licencia
Este proyecto está bajo la licencia MIT. Las herramientas de terceros utilizadas de forma interna (como chdman, etc.) pertenecen a sus respectivos desarrolladores y se distribuyen bajo sus propias condiciones de uso comunitario.

desarrollado con 💖 para la comunidad de preservación de videojuegos.
