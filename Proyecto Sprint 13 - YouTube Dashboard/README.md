# 📊 Proyecto Sprint 13 – Dashboard de Tendencias de YouTube  
**Bootcamp de Data Analytics – TripleTen**

---

## 📷 Vista previa del dashboard

<img width="993" height="396" alt="dashboard_preview" src="https://github.com/user-attachments/assets/c56f7439-e18f-4567-8f18-e4306715b653" />

📊 **Vista previa del dashboard interactivo** desarrollado en Tableau Public, donde se visualizan las tendencias históricas de videos en YouTube por categoría y país, incluyendo análisis temporal, distribución geográfica y comparaciones relativas.  
El dashboard completo puede explorarse de forma interactiva mediante el enlace a Tableau Public incluido más abajo.

---

## 📌 Descripción del proyecto

En este proyecto se desarrolló un **dashboard interactivo en Tableau** para analizar el historial de tendencias de videos en YouTube, con el objetivo de **automatizar el análisis semanal de contenido en tendencia** y apoyar la toma de decisiones en campañas de marketing digital.

El dashboard permite explorar cómo evolucionan las tendencias de videos a lo largo del tiempo, cómo se distribuyen por país y categoría, y qué tipos de contenido son particularmente populares en regiones específicas, como Estados Unidos.

Este proyecto está orientado a **usuarios de negocio** (gerentes de planificación de contenido publicitario), por lo que se priorizó la claridad visual, la interactividad y la facilidad de interpretación.

---

## 🎯 Objetivo del proyecto

Crear un dashboard que permita responder de forma rápida y visual a preguntas clave del negocio, tales como:

- ¿Qué categorías de videos aparecen con mayor frecuencia en tendencias?
- ¿Cómo se distribuyen las tendencias entre distintos países?
- ¿Qué categorías son especialmente populares en Estados Unidos?
- ¿Existen diferencias relevantes entre países en términos de contenido en tendencia?

---

## 📂 Conjunto de datos utilizado

Se trabajó con una tabla de agregación proporcionada por el equipo de ingeniería:

**`trending_by_time.csv`**

Estructura del dataset:
- `record_id`: identificador único del registro
- `region`: país o región geográfica
- `trending_date`: fecha y hora en que el video fue tendencia
- `category_title`: categoría del video
- `videos_count`: número de videos en tendencia

Los datos se actualizan con una frecuencia diaria y representan el historial de tendencias por fecha, país y categoría.

---

## 🧩 Estructura del dashboard

El dashboard fue diseñado siguiendo un borrador funcional y contiene los siguientes elementos:

### 🔹 Filtros globales
- Filtro de **fecha y hora**
- Filtro de **país**

Ambos filtros afectan a todos los gráficos del dashboard.

### 🔹 Visualizaciones principales

- **Historial de tendencias (valores absolutos)**  
  Gráfico de área que muestra el número de videos en tendencia a lo largo del tiempo, segmentado por categoría.

- **Historial de tendencias (%)**  
  Gráfico de área que muestra la participación porcentual de cada categoría respecto al total de videos en tendencia.

- **Tendencias de videos por país**  
  Gráfico de pastel que muestra la distribución relativa de videos en tendencia por país.

- **Tendencias por país y categoría**  
  Tabla de valores absolutos con formato condicional, que permite comparar categorías entre regiones.

---

## 🛠️ Herramientas y tecnologías utilizadas

- Tableau Public
- Análisis visual de datos
- Dashboards interactivos
- Storytelling con datos

---

## 📈 Principales hallazgos

- La categoría **Entertainment** domina consistentemente las tendencias en la mayoría de las regiones.
- Existen diferencias claras entre países en la distribución de categorías populares.
- Estados Unidos presenta patrones de consumo distintos en comparación con otras regiones, especialmente en categorías como **Music** y **People & Blogs**.
- El análisis temporal permite identificar picos y cambios en las tendencias a lo largo del periodo analizado.

---

## 🔗 Dashboard interactivo

El dashboard completo puede consultarse públicamente en Tableau Public:

👉 https://public.tableau.com/app/profile/oscar.aranda7717/viz/YouTube_Trending_Analysis/YouTubeTrends

---

## 📂 Archivos del proyecto

- 📊 `trending_by_time.csv` – Dataset utilizado para el dashboard
- 📄 `Dashboard_de_Analisis_de_Tendencias_de_YouTube.pdf` – Presentación ejecutiva del análisis
- 📘 `README.md` – Documentación del proyecto

---

## ✅ Estado del proyecto

✔ Dashboard publicado y accesible públicamente  
✔ Requisitos técnicos cumplidos  
✔ Análisis visual alineado a objetivos de negocio  

---

## 🧠 Nota final

Este proyecto demuestra la capacidad de **traducir datos agregados en visualizaciones claras**, construir dashboards orientados a negocio y comunicar insights de manera efectiva, facilitando la toma de decisiones en entornos de marketing digital basados en datos.
