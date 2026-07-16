---
name: diseno-guias-2027
description: Reglas de diseño, hojas de estilos CSS y estándares de distribución visual para la creación de guías de estudio y talleres del ciclo 2027 en formato de dos columnas y diagramación Letter.
---
# Directrices de Diseño y Estructura: Guías de Estudio 2027

Este Skill documenta de manera precisa las decisiones estéticas, cromáticas, de distribución y de maquetación técnica para que todas las futuras guías de estudio y talleres prácticos mantengan una calidad gráfica premium y uniforme.

---

## 1. Paleta Cromática y Tipografía (Estilo Red Block)
- **Color de Identidad Primario**: Rojo Premium (`#e53935`).
- **Color de Texto y Títulos**: Gris carbón oscuro (`#263238`).
- **Fuentes Tipográficas**:
  - Títulos principales, secciones y cabeceras: `'Fredoka', sans-serif` (Google Fonts).
  - Cuerpo de texto y fórmulas explicativas: `'Inter', sans-serif` (Google Fonts).
  - Fórmulas matemáticas avanzadas: Siempre renderizadas en LaTeX usando la biblioteca MathJax.
- **Secciones del Documento**:
  - Utilizar encabezados `.section-header-red` que incluyan un indicador numérico rojo (`.section-badge-red`) y una línea de borde inferior roja de `2.5px solid #e53935`.

## 2. Tipos de Cajas de Contenido (Paleta Pastel Cohesiva)
- **Teoría General y Definiciones**:
  - Fondo azul pastel (`#f0f8ff`) con bordes en azul claro (`#add8e6`).
- **Operaciones Resueltas, Notas Matemáticas o Alertas**:
  - Fondo amarillo/naranja pastel (`#fffde7`) con bordes en amarillo (`#ffe082`).
- **Tarjetas de Problemas de Taller**:
  - Fondo blanco puro (`#ffffff`) con bordes grises muy finos (`#cfd8dc`). Evitar fondos de colores en las cajas de taller cuando contengan imágenes para no saturar visualmente el diseño.

## 3. Maquetación y Distribución de Páginas (Carta / Letter)
- **Dimensiones Exactas**: Cada página física se define con una clase `.page` de `width: 22cm` y `height: 28cm`, con desbordamiento oculto (`overflow: hidden`) para prevenir páginas adicionales accidentales en blanco al imprimir a PDF.
- **Consolidación del Taller de Práctica**:
  - El taller se diseña en una maquetación simétrica a **dos columnas** (`display: grid; grid-template-columns: 1.1fr 0.9fr; gap: 22px;`).
  - **Evitar la fragmentación**: Todas las preguntas del taller deben agruparse para encajar de manera holgada y completa en una sola página física.
  - **Respiración Visual (Breathing Room)**: Dar espacio entre las preguntas usando márgenes inferiores amplios (`margin-bottom: 18px` en `.taller-question`) y alturas de tarjetas generosas para evitar que los ejercicios se sientan apretados o compactados ("apeñuscados").

## 4. Estándar para Ilustraciones e Imágenes con IA
- Las imágenes explicativas e ilustrativas para problemas de la vida real deben tener un acabado **realista 3D detallado** (estilo libro escolar moderno de alta calidad).
- Deben estar aisladas sobre un fondo blanco puro (`#ffffff`) para mezclarse de forma fluida con las tarjetas blancas.
- **Distribución de las imágenes**:
  - No ubicar imágenes a los lados de los textos si las columnas son estrechas.
  - Colocar las imágenes grandes (**120px** de ancho y alto) y **completamente centradas arriba del enunciado del problema**, logrando una composición vertical limpia y estructurada.
