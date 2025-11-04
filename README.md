# PEC2 –  Análisis de Técnicas de Visualización

Este proyecto forma parte de la **PEC2 de la asignatura M2.890 – Visualización de datos** del Máster en Ciencia de Datos de la UOC.

El objetivo es realizar un **Análisis de Técnicas de Visualización** del mercado de los videojuegos utilizando el dataset `dataset_vgsales.csv`, aplicando **tres técnicas de visualización** para extraer conocimiento sobre el rendimiento de plataformas y géneros.

---

## Entorno de trabajo y dependencias

| Elemento          | Descripción |
|-------------------|-------------|
| **Lenguaje**      | R |
| **Documento principal** | R Markdown → HTML interactivo (`M2.859_Visualizacion_PEC2.Rmd`) |
| **Librerías clave** | `ggplot2`, `dplyr`, `networkD3`, `tidyverse`, `scales` |
| **Dataset utilizado** | `data/dataset_vgsales.csv` |

---

## Técnicas de Visualización

| Técnica | Objetivo | Variables |
|---------|----------|-----------|
| **1. Sankey Diagram** | Representar el flujo de ventas globales desde los *géneros* hacia las *compañías* (agrupando plataformas por marca: Sony, Nintendo, Xbox, etc.) | `Genre → Company` (Global_Sales) |
| **2. Boxplot** | Analizar la distribución, mediana y dispersión de ventas globales por compañía. Se aplica escala logarítmica para mejorar la lectura. | `Company` vs `Global_Sales (log10)` |
| **3. Convex Hull** | Delimitar el espacio de ventas combinadas entre Norteamérica (NA) y Europa (EU) para cada compañía, mostrando el rango competitivo de cada una. | `NA_Sales`, `EU_Sales` agrupado por `Company` |

---

## Estructura del Proyecto

El dataset empleado se encuentra en la carpeta `data/`.

Las visualizaciones **HTML** con gráficos interactivos se encuentra en la carpeta `docs/`.

El código para generar las visualizaciones se ha realizado en lenguaje R, y se encuentra en la carpeta `scripts/`.

---

## Autor

**Francisco Heredia Mañas**

---
