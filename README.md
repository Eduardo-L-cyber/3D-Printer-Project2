# 3D-Printer-Project

Este repositorio es una guía centralizada y un contenedor de recursos para la configuración, optimización y control de impresoras 3D. Aquí encontrarás archivos específicos para **Marlin**, **Klipper** y **OctoPrint**, junto con la documentación necesaria para implementarlos.

---
# 3D-Printer-Project

Este repositorio es una guía centralizada y un contenedor de recursos para la configuración, optimización y control de impresoras 3D. Aquí encontrarás archivos específicos para **Marlin**, **Klipper** y **OctoPrint**, junto con la documentación necesaria para implementarlos.

---

## 📥 Cómo descargar este proyecto

Si eres nuevo en GitHub, aquí tienes dos formas de obtener estos archivos:

### Opción A: Descargar todo el proyecto (Recomendado)
Para bajar todas las carpetas, configuraciones y manuales de una sola vez:
1. Haz clic en el botón verde que dice **"<> Code"** (está en la parte superior derecha).
2. En el menú desplegable, selecciona **"Download ZIP"**.
3. Descomprime el archivo en tu computadora y ¡listo!

### Opción B: Descargar un archivo específico (como el .rar de Marlin)
Si solo necesitas un archivo puntual:
1. Haz clic sobre el nombre del archivo (ejemplo: `Marlin-2.1.2.7_BTT Octopus v1.1.rar`).
2. En la siguiente pantalla, busca el botón **"Download"** (o el icono de la flecha hacia abajo) en la parte derecha.
3. El archivo se guardará directamente en tu carpeta de descargas.

---

## 💡 Conceptos Básicos

Para dominar la configuración de tu impresora, es fundamental entender la diferencia entre el hardware de control y el de procesamiento:

* **MCU (Microcontroller Unit):** Es la "placa" de la impresora (en este caso, la **BTT Octopus v1.1**). Es el componente que recibe las señales eléctricas y controla físicamente los motores, calentadores y sensores. 
* **Host (Servidor):** Es un ordenador de placa única, como la **Orange Pi Zero 3** o una Raspberry Pi. Actúa como el "cerebro" avanzado que procesa interfaces web y cálculos complejos que la MCU no podría manejar por sí sola.

---

## 🛠️ Guía de Selección: ¿Qué sistema elegir?

Dependiendo de tu hardware disponible y tus objetivos, puedes elegir entre estas tres opciones principales:

### 1. Marlin Firmware
Es el estándar de la industria, un firmware que corre directamente en la MCU.
* **Cuándo usarlo:** Úsalo si **no cuentas con un Host** (como una Orange Pi o Raspberry Pi). Es ideal para quienes buscan una experiencia tradicional, estable y que no dependa de una red WiFi o servidores externos para imprimir.

### 2. Klipper
Un ecosistema híbrido donde el Host hace el trabajo pesado y la MCU ejecuta los movimientos.
* **Cuándo usarlo:** Úsalo si tienes una **Orange Pi Zero 3** o similar y buscas **máxima velocidad y calidad**. Es la mejor opción si quieres editar la configuración de tu impresora rápidamente sin tener que compilar y flashear el firmware cada vez que hagas un cambio.

### 3. OctoPrint
Una interfaz web potente que se comunica con impresoras que corren Marlin.
* **Cuándo usarlo:** Úsalo si tu **MCU es muy antigua** (placas de 8 bits) o limitada, pero quieres modernizarla añadiendo control remoto por navegador, gestión de cámaras y plugins, manteniendo la base de Marlin.

---

## 📁 Estructura del Repositorio

* **/Archivos Klipper:** Archivos de configuración (`printer.cfg`) optimizados para la placa BTT Octopus.
* **/Documentacion de Klipper:** Guías técnicas para la instalación y calibración del firmware.
* **Marlin-2.1.2.7_BTT Octopus v1.1.rar:** Paquete de firmware Marlin pre-configurado para la placa Octopus.
* **/Manuales:** Guías detalladas para la implementación de OctoPrint y Marlin (en desarrollo).

---

## 🚀 Instalación y Uso

1.  **Para Marlin:** Descomprime el archivo `.rar` y sigue las instrucciones del manual de flasheo incluido.
2.  **Para Klipper:** Instala el sistema operativo en tu Host y vincula los archivos de la carpeta correspondiente.
3.  **Para OctoPrint:** Consulta la guía de instalación para habilitar el servidor en tu Orange Pi.

---
*Mantenido por Eduardo-L-cyber*
