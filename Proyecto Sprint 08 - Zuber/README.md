# 🚕 Proyecto Sprint 8 – Zuber  
## Análisis de Movilidad Urbana y Clima en Chicago

**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción del proyecto
Zuber es una empresa de transporte que busca introducirse en el mercado de movilidad urbana en la ciudad de Chicago. Para lograr una entrada estratégica y competitiva, la empresa necesita comprender los patrones de viaje existentes, identificar zonas de alta demanda y analizar cómo factores externos, como el clima, influyen en la duración de los trayectos.

En este proyecto se analizan datos reales de viajes en taxi correspondientes a noviembre de 2017, integrando información extraída mediante consultas SQL y análisis exploratorio en Python, con el objetivo de generar insights accionables para la etapa inicial de operación de Zuber.

---

## 🎯 Objetivo del proyecto
Analizar patrones de movilidad urbana en Chicago y evaluar el impacto del clima en la duración de los viajes, con el fin de identificar oportunidades estratégicas y operativas para la entrada de Zuber al mercado.

---

## 📂 Conjuntos de datos utilizados
Se trabajó con datos extraídos previamente mediante consultas SQL y analizados posteriormente en Python:

- **project_sql_result_01.csv** – número de viajes por compañía de taxis (15 y 16 de noviembre de 2017)
- **project_sql_result_04.csv** – promedio de viajes por barrio de destino durante noviembre de 2017
- **project_sql_result_07.csv** – duración de viajes desde el barrio Loop hasta el Aeropuerto Internacional O’Hare, incluyendo condiciones climáticas

---

## 🧩 Etapas del análisis
🔹 **Exploración y validación de datos**  
- Importación de archivos CSV  
- Revisión de estructura y tipos de datos  

🔹 **Análisis exploratorio de datos (EDA)**  
- Identificación de las empresas de taxis con mayor número de viajes  
- Identificación de los 10 barrios con más finalizaciones de recorrido  
- Visualización de patrones de viajes por empresa y por barrio  

🔹 **Análisis del impacto del clima**  
- Comparación de la duración de trayectos bajo distintas condiciones climáticas  
- Enfoque específico en los viajes desde Loop hasta el Aeropuerto O’Hare  

🔹 **Pruebas de hipótesis estadísticas**  
- Evaluación de diferencias en la duración promedio de los viajes en sábados lluviosos  

---

## 📊 Visualizaciones realizadas
- Gráficos de barras para comparar el número de viajes por empresa de taxis  
- Gráficos de barras para identificar los 10 barrios con mayor número de finalizaciones  
- Diagramas de caja para analizar la distribución de la duración de los trayectos según las condiciones climáticas  

---

## 🧪 Prueba de hipótesis
**Hipótesis planteada:**  
> *La duración promedio de los viajes desde el Loop hasta el Aeropuerto Internacional O’Hare cambia los sábados lluviosos.*

Para su evaluación se aplicaron:
- **Prueba de Levene**, para verificar la homogeneidad de varianzas  
- **Prueba t de Student**, para comparar las medias  

Nivel de significancia utilizado: **α = 0.05**

---

## 📈 Resultados clave
- Los barrios de **Loop**, **River North** y **Streeterville** concentran la mayor demanda de viajes, destacando Loop como zona estratégica.
- **Flash Cab** lidera el mercado en número de viajes durante los días analizados, reflejando el dominio de empresas establecidas.
- Los trayectos realizados bajo condiciones climáticas adversas presentan una mayor duración promedio.
- La prueba t de Student mostró una diferencia estadísticamente significativa en la duración de los viajes durante sábados lluviosos, específicamente en la ruta Loop → O’Hare.

---

## 🧠 Conclusiones y recomendaciones
El análisis evidencia que el clima y la localización influyen significativamente en la duración y frecuencia de los viajes en taxi en Chicago. En particular, los sábados lluviosos incrementan la duración de los trayectos desde Loop hasta el Aeropuerto O’Hare.

**Recomendaciones para Zuber:**
- Priorizar el inicio de operaciones en barrios de alta demanda como Loop y River North.
- Ajustar la disponibilidad de flota en días lluviosos para mitigar retrasos.
- Incorporar información climática en la aplicación para mejorar las estimaciones de tiempo de llegada (ETA) y la experiencia del usuario.

---

## 🛠️ Herramientas y tecnologías utilizadas
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- SciPy  
- SQL (extracción de datos)  

---

## 📂 Archivos del proyecto
📓 **Notebook principal:**  
- `notebook - Zuber.ipynb`

---

## ✅ Estado del proyecto
- ✔ Proyecto completado  
- ✔ Análisis exploratorio documentado  
- ✔ Pruebas estadísticas aplicadas  

---

## 🧠 Nota final
Este proyecto demuestra la capacidad de integrar datos provenientes de consultas SQL con análisis exploratorio y pruebas estadísticas en Python, generando recomendaciones estratégicas basadas en evidencia para la toma de decisiones en el sector de movilidad urbana.
