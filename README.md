# Visualización de Modelo RYB/WK con Corrección por Luminancia

Este proyecto permite analizar y visualizar cómo los colores de una imagen .jpeg se descomponen en los modelos **RYB (Rojo-Amarillo-Azul)** y **WK (Blanco-Negro)**, ajustando la relación entre ambos en función de la **luminancia corregida (canal L)**, de acuerdo con principios del comportamiento pigmentario.

---

## 🔍 Características

- 📷 Carga de imágenes .jpeg desde el navegador.
- 🎨 Conversión por píxel del modelo **RGB** a:
  - RYB: usando lógica pigmentaria con refinamiento.
  - WK: estimado a partir de la luminancia.
- ⚖️ Determinación del **modelo dominante (RYB o WK)** según la luminancia corregida.
- 📊 Visualización dinámica por píxel con **gráficos circulares (pie chart)**:
  - Subcomponentes RYB: % Rojo, % Amarillo, % Azul.
  - Subcomponentes WK: % Blanco, % Negro.
  - Relación integrada RYB/WK.
- 🌕 Corrección interactiva del canal **L** (Luminancia) mediante un slider.
- 🎛️ Todo embebido en un único archivo `.html` funcional desde Live Server.

---

## 📁 Estructura del Proyecto

```
.
├── index.html       # App completa, ejecutable desde Live Server
├── style.css        # (Opcional) Estilos personalizados para visuales suaves
├── README.md        # Documentación del proyecto
```

---

## 🚀 Cómo usar

1. Abrí el proyecto con **Live Server** (Visual Studio Code recomendado).
2. Seleccioná una imagen `.jpeg` desde tu dispositivo.
3. Pasá el cursor sobre la imagen para visualizar el análisis de cada píxel.
4. Ajustá el **factor de luminancia** con el slider para modificar la relación RYB/WK.
5. Observá el gráfico circular que muestra la proporción de pigmentos por píxel.

---

## ⚗️ Modelo de Relación Pigmentaria

- En **luminancias intermedias**, predomina el modelo RYB.
- En **luminancias muy bajas o altas**, domina el modelo WK.
- La transición entre ambos se calcula en tiempo real, ponderando cada componente.

---

## 🧠 Pendientes / Ideas Futuras

- Agregar modo de visualización por regiones.
- Exportar análisis como JSON o imagen procesada.
- Ajustes avanzados sobre curva de corrección L.
- Soporte para PNG y otros formatos con canal alpha.

---

## 🖼️ Créditos Visuales

Este proyecto utiliza lógica personalizada para interpretar modelos pigmentarios a partir de RGB, y fue desarrollado como herramienta didáctica para análisis visual y de percepción del color.

---

## ⚙️ Requisitos

- Navegador moderno (Chrome, Firefox, Edge, etc.)
- Extensión Live Server (si usás VSCode)

---

## 👨‍💻 Autor

Desarrollado por [Tu Nombre o Alias] — 2025  
Proyecto con fines educativos / exploratorios de teoría del color.
