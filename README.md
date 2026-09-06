# Laboratorio de Realidad Virtual: Entorno Industrial XR Multiplataforma 🏭🥽

## Descripción del Proyecto
Este repositorio contiene el desarrollo de un entorno de Realidad Extendida (XR) multiplataforma basado en la web, creado como parte de la asignatura de Realidad Virtual del programa de Ingeniería Mecatrónica de la Universidad Militar Nueva Granada. 

El proyecto utiliza el framework **A-Frame** (basado en HTML y WebGL) para visualizar escenarios interactivos en múltiples dispositivos sin necesidad de software propietario, aplicando conceptos de digitalización de la Industria 4.0.

## Características de la Escena
El entorno virtual se compone de dos secciones principales de acuerdo con la guía de laboratorio:

1. **Línea de Empaquetado Automatizada (Primitivas):** 
   Diseño de un sistema industrial construido mediante jerarquías espaciales y primitivas geométricas nativas de A-Frame (`<a-box>`, `<a-cylinder>`, `<a-sphere>`, `<a-plane>`). El sistema incluye:
   * Banda transportadora con cajas de producto.
   * Arco de sensores y escáner láser.
   * Brazo robótico tipo "pick and place".
   * Panel de control con interfaz HMI.

2. **Integración de Modelo CAD Externo:** 
   Visualización inmersiva de un modelo industrial (`floordyer.glb`). El modelo fue exportado desde software CAD y procesado externamente para optimizar su geometría (reducción de polígonos) asegurando que su peso sea inferior a 25 MB. Esto garantiza un alto rendimiento gráfico y baja latencia en dispositivos móviles y visores VR.

## Tecnologías Utilizadas
* **A-Frame & WebXR:** Renderizado 3D y soporte de realidad inmersiva.
* **HTML5:** Estructura de la escena.
* **SolidWorks / Blender:** Modelado mecánico, aplicación del modificador *Decimate* y exportación a formato `.glb`.
* **GitHub Pages:** Despliegue en la nube para acceso público.

## Cómo Visualizar el Proyecto
El entorno está alojado públicamente y es accesible desde cualquier navegador moderno compatible con WebXR.

🔗 **[Haz clic aquí para ingresar a la Planta Industrial XR](https://mariluuu2633.github.io/Realidad-Virtual-XR/)** *(Nota: Inserta tu enlace real aquí)*

### Instrucciones por Plataforma:
* 💻 **PC de Escritorio:** Haz clic y arrastra el ratón para mirar alrededor. Usa las flechas del teclado o las teclas `W A S D` para desplazarte por la planta.
* 📱 **Smartphone (AR / VR):** 
  * *Visualización estándar:* Mueve el teléfono físicamente (sensores IMU) para observar el entorno.
  * *Modo VR:* Toca el ícono de las gafas (esquina inferior derecha) e inserta el celular en un visor tipo Cardboard.
* 🥽 **Visor Meta Quest 3:** Abre el navegador integrado del visor, ingresa a la URL y selecciona el botón "Enter VR" para disfrutar de la experiencia inmersiva a escala real con seguimiento de cabeza y manos.

## Estructura del Repositorio
```text
📦 xr-industrial-lab
┣ 📂 models
┃ ┗ 📜 floordyer.glb     # Modelo CAD optimizado (peso < 25MB)
┗ 📜 index.html          # Código principal de la escena y jerarquías
