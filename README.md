# 🎨 Lo Mejor del Arte: Galería con Inteligencia Artificial

![Estado del Proyecto](https://img.shields.io/badge/Estado-Terminado-success)
![Tecnología](https://img.shields.io/badge/AI-Teachable_Machine-blue)
![Stack](https://img.shields.io/badge/Web-HTML%20%7C%20CSS%20%7C%20JS-orange)

Este proyecto es una aplicación web interactiva que utiliza **Visión por Computadora (Computer Vision)** para identificar obras de arte famosas en tiempo real mediante la cámara del dispositivo. Su objetivo es funcionar como un guía de museo inteligente, proporcionando información histórica y estilística al instante.

---

## 📹 Video Demostrativo

Explicación del funcionamiento, demostración en vivo y conclusiones del proyecto (2 min).

[![Ver Video en YouTube](https://img.youtube.com/vi/TU_ID_DEL_VIDEO_AQUI/0.jpg)](https://www.youtube.com/watch?v=TU_LINK_DEL_VIDEO)

> **Haz clic en la imagen o [aquí](PEGAR_TU_LINK_DE_YOUTUBE_AQUI) para ver la presentación.**

---

## 🚀 Descripción y Objetivos

### El Problema
En los museos o al estudiar arte, a menudo vemos una pintura pero desconocemos su contexto, autor o la técnica utilizada.

### La Solución
Una interfaz web accesible que, mediante Inteligencia Artificial, reconoce la pintura que se le muestra y despliega una ficha técnica con:
* Nombre de la obra.
* Artista.
* Descripción detallada.
* Época o movimiento artístico.

### Objetivos Principales
1.  Implementar un modelo de clasificación de imágenes eficiente usando **Teachable Machine**.
2.  Crear una interfaz de usuario ("Frontend") inmersiva con temática de galería de arte.
3.  Demostrar el uso de modelos híbridos (detección de obra específica vs. detección de estilo de autor).

---

## 🧠 Sobre el Modelo de IA (Teachable Machine)

El núcleo del proyecto es un modelo de red neuronal entrenado con **Google Teachable Machine** y exportado a **TensorFlow.js**.

### Estrategia Híbrida de Entrenamiento
Para lograr una mayor precisión y utilidad educativa, se tomó la decisión técnica de crear un **modelo híbrido** con dos tipos de clases:

1.  **Clases de Granularidad Fina (Obras Específicas):**
    * Se entrenaron clases específicas para obras maestras icónicas (ej: *La Noche Estrellada*, *Guernica*).
    * **Resultado:** Al detectar estas obras, el sistema muestra datos exactos de esa pintura.

2.  **Clases de Granularidad Gruesa (Estilo de Autor):**
    * Se entrenaron clases genéricas con múltiples obras de un mismo pintor (ej: *Vincent van Gogh*, *Pablo Picasso*).
    * **Resultado:** Si el usuario muestra una obra del pintor que no está en la lista específica, el modelo reconoce el "estilo" del autor y ofrece información biográfica general.

**Total de Clases:** [NÚMERO] clases entrenadas.
**Precisión:** Umbral de confianza configurado al 85% para evitar falsos positivos.

---

## 🛠️ Tecnologías Utilizadas

* **Google Teachable Machine:** Para el entrenamiento y exportación del modelo (TensorFlow.js).
* **HTML5:** Estructura semántica de la página.
* **CSS3:** Diseño responsivo, estilo "Dark Academy/Museo", gradientes y efectos visuales.
* **JavaScript (Vanilla):** Lógica del cliente, manejo del DOM, integración con la webcam y función de "congelar imagen".
* **Visual Studio Code + Live Server:** Entorno de desarrollo.

---

## 💻 Instalación y Ejecución

Para probar este proyecto en tu computadora local:

1.  **Clonar el repositorio:**
    ```bash
    git clone [https://github.com/TU_USUARIO/TU_REPOSITORIO.git](https://github.com/TU_USUARIO/TU_REPOSITORIO.git)
    ```
2.  **Abrir la carpeta** en Visual Studio Code.
3.  **Instalar la extensión "Live Server"** en VS Code (es necesario para que el navegador tenga permisos de usar la cámara).
4.  Hacer clic derecho en el archivo `index.html` y seleccionar **"Open with Live Server"**.
5.  Dar permisos al navegador para usar la cámara web.

---

## 📄 Proceso de Desarrollo y Decisiones Técnicas

1.  **Recolección de Datos:** Se recopilaron imágenes de alta resolución de museos digitales y Google Arts & Culture.
2.  **Entrenamiento:** Se realizaron iteraciones para corregir el sesgo (bias) cuando el fondo de las imágenes confundía al modelo.
3.  **Interfaz:** Se optó por un diseño oscuro para resaltar los colores de las pinturas. Se añadió un botón de **"Congelar/Apagar"** para permitir al usuario detener la predicción y leer la información con calma, una característica clave para la usabilidad.

---

## 🎓 Conclusiones

Este proyecto demuestra cómo las herramientas "No-Code" o "Low-Code" como Teachable Machine pueden integrarse con desarrollo web tradicional para crear aplicaciones educativas potentes. El modelo híbrido resultó ser la estrategia más efectiva para manejar tanto obras muy famosas como el estilo general de un artista.

---

**Desarrollado por:** [TU NOMBRE COMPLETO]  
**Materia:** [NOMBRE DE LA MATERIA]  
**Fecha:** Noviembre 2025
