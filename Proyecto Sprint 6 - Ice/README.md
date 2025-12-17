# 🎮 Proyecto Sprint 6 – Ice  
## Análisis de Éxito de Videojuegos y Patrones de Venta Globales

**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción del proyecto
Ice es una tienda online que vende videojuegos a nivel mundial. Para planificar campañas publicitarias efectivas, la empresa necesita identificar **patrones que determinan el éxito de un videojuego**, considerando factores como ventas históricas, plataformas, géneros, reseñas de usuarios y expertos, y diferencias regionales.

En este proyecto se analizan datos históricos hasta el año 2016, con el objetivo de **extraer insights que ayuden a tomar decisiones estratégicas para el año 2017**.

---

## 🎯 Objetivo del proyecto
Identificar patrones de éxito en la industria de los videojuegos mediante el análisis de ventas, reseñas, plataformas, géneros y regiones, y evaluar hipótesis estadísticas relacionadas con las calificaciones de usuarios.

---

## 📂 Conjunto de datos utilizado
- `games.csv` – información histórica de videojuegos, incluyendo ventas regionales, plataformas, géneros, calificaciones y clasificación ESRB.

### Principales variables
- `Name` – nombre del videojuego  
- `Platform` – plataforma  
- `Year_of_Release` – año de lanzamiento  
- `Genre` – género  
- `NA_sales`, `EU_sales`, `JP_sales`, `Other_sales` – ventas regionales (millones USD)  
- `Critic_Score` – calificación de críticos (0–100)  
- `User_Score` – calificación de usuarios (0–10)  
- `Rating` – clasificación ESRB  

---

## 🧩 Etapas del análisis

### 🔹 Etapa 1: Exploración y preparación de datos
- Normalización de nombres de columnas
- Conversión de tipos de datos
- Identificación y tratamiento de valores ausentes
- Manejo de valores especiales como `"TBD"` en calificaciones
- Cálculo de ventas globales por juego a partir de ventas regionales

---

### 🔹 Etapa 2: Análisis exploratorio de datos (EDA)
- Análisis del número de lanzamientos por año
- Estudio del ciclo de vida de las plataformas
- Identificación de plataformas líderes y en declive
- Selección de un período relevante para proyectar tendencias hacia 2017
- Comparación de ventas globales por plataforma mediante diagramas de caja
- Evaluación de la relación entre reseñas (usuarios y críticos) y ventas

---

### 🔹 Etapa 3: Análisis por género
- Distribución de videojuegos por género
- Identificación de géneros más rentables
- Comparación entre géneros con ventas altas y bajas

---

### 🔹 Etapa 4: Perfil de usuario por región
Se construyó un perfil para cada región:

- **Norteamérica (NA)**
- **Europa (EU)**
- **Japón (JP)**

Para cada región se analizaron:
- Las cinco plataformas principales
- Los cinco géneros más populares
- El impacto de la clasificación ESRB en las ventas

---

### 🔹 Etapa 5: Pruebas de hipótesis
Se evaluaron las siguientes hipótesis estadísticas:

1. Las calificaciones promedio de los usuarios para **Xbox One** y **PC** son iguales.
2. Las calificaciones promedio de los usuarios para los géneros **Acción** y **Deportes** son diferentes.

Se utilizaron **pruebas t de Student**, definiendo explícitamente las hipótesis nula y alternativa, así como el nivel de significancia.

---

## 🛠️ Herramientas y tecnologías utilizadas
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **SciPy (stats)**
- Análisis exploratorio de datos
- Análisis estadístico inferencial

---

## 📈 Resultados clave
- La industria de los videojuegos muestra un crecimiento sostenido hasta 2008–2009, seguido de un declive en lanzamientos.
- Las plataformas presentan ciclos de vida cortos (6–7 años).
- No se identificaron plataformas con crecimiento sostenido claro hacia 2017 dentro del dataset.
- Las reseñas de críticos presentan una **correlación moderada** con las ventas (ej. PS3 ≈ 0.43).
- Las reseñas de usuarios muestran una **correlación débil** con las ventas.
- Existen **diferencias significativas entre regiones** en cuanto a plataformas, géneros y preferencias ESRB.

---

## 🧠 Conclusiones
El análisis confirma que el éxito de un videojuego depende de múltiples factores, incluyendo plataforma, región, género y recepción crítica. Las preferencias varían notablemente entre Norteamérica, Europa y Japón, lo que refuerza la necesidad de **estrategias de marketing regionalizadas**.

Las pruebas estadísticas muestran que:
- Existen diferencias significativas en las calificaciones promedio entre Xbox One y PC.
- No hay evidencia suficiente para afirmar diferencias entre las calificaciones promedio de los géneros Acción y Deportes.

Estos hallazgos permiten orientar decisiones estratégicas en un mercado dinámico y altamente competitivo.

---

## 📂 Archivos del proyecto
- 📓 **Notebook principal:**  
  `notebook - Ice.ipynb`

---

### ✅ Estado del proyecto
✔ Proyecto completado  
✔ Análisis exploratorio y estadístico documentado  

---

## 🔗 Enlace al repositorio
📎 https://github.com/utsa2004/proyectos-bootcamp-data-analyst-tripleten/tree/main/Proyecto%20Sprint%206%20-%20Ice

---

## 🧠 Nota final
Este proyecto demuestra la capacidad de analizar datos históricos complejos, identificar patrones de mercado, realizar análisis regional y aplicar pruebas estadísticas para apoyar decisiones estratégicas en la industria de los videojuegos.

