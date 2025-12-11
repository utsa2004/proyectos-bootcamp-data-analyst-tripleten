# 🚕 Proyecto Sprint 8 – Zuber: Análisis de Movilidad Urbana en Chicago  
**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción del proyecto
Este proyecto analiza patrones de movilidad en la ciudad de Chicago durante noviembre de 2017 con el fin de comprender factores que influyen en los viajes en taxi y generar recomendaciones estratégicas para **Zuber**, una empresa que busca introducirse en el mercado de transporte urbano.

El análisis integra:
- Datos meteorológicos  
- Datos de viajes por empresa  
- Información de barrios de destino  
- Duración de trayectos bajo diferentes condiciones climáticas  

A partir de consultas SQL y análisis exploratorio en Python, se estudian tendencias relevantes para entender demanda, variabilidad en los trayectos y diferencias entre empresas competidoras.

---

## 🎯 Objetivo del proyecto
Identificar factores que influyen en el comportamiento de los usuarios de servicios de transporte urbano y generar recomendaciones estratégicas para Zuber basadas en evidencia.

---

## 📂 Datasets utilizados
Se trabajó con tres conjuntos de datos extraídos mediante SQL:

- **chicago1:** viajes por empresa de taxis  
- **chicago2:** viajes por barrio de destino  
- **chicago3:** duración de trayectos entre Loop → Aeropuerto O’Hare, con condiciones climáticas asociadas  

---

## 🧠 Metodología

### **1. Preparación y revisión de datos**
- Importación de datasets  
- Validación de tipos de datos  
- Revisión de valores atípicos  
- Estandarización de columnas y categorías  

### **2. Análisis exploratorio (EDA)**
- Comparación del número de viajes por empresa  
- Identificación de los 10 barrios con más finalizaciones de viajes  
- Evaluación de patrones en fechas específicas  
- Relación entre clima y duración de trayectos  

### **3. Visualización**
Se generaron gráficos para:
- Cantidad de viajes por compañía  
- Barrios más visitados  
- Distribución de duraciones bajo distintas condiciones climáticas  
- Comparación Loop → O’Hare  

### **4. Pruebas de hipótesis**
Para evaluar si el clima afecta significativamente la duración de los viajes en la ruta Loop → O’Hare se aplicaron:

- **Prueba de Levene:** evaluación de igualdad de varianzas  
- **Prueba t de Student:** comparación de medias entre días lluviosos vs. no lluviosos  

Resultado clave:  
➡️ La duración promedio en días lluviosos fue **significativamente mayor** (p ≈ 0.0000), lo cual confirma el impacto del clima.

---

## 📊 Hallazgos principales

### **1. Zonas de alta demanda**
Barrios como **Loop**, **River North** y **Streeterville** concentran gran parte de los viajes.  
Loop destaca con más de **10,700 viajes promedio**, posicionándose como punto estratégico para operaciones iniciales.

### **2. Liderazgo de empresas consolidadas**
En los días analizados:
- **Flash Cab** fue líder absoluto en número de viajes  
- Zuber aún no aparece entre las empresas más activas  

Esto evidencia la necesidad de una estrategia inicial sólida para ganar visibilidad.

### **3. Impacto del clima en la duración de trayectos**
- Los días lluviosos presentan **mayor duración mediana**  
- El clima afecta la ruta Loop → O’Hare con significancia estadística  
- En días con buen clima se observan más valores atípicos y mayor dispersión  

### **4. Influencia del clima (ruta Loop → O'Hare)**
Resultados estadísticos:
- ✔ Igualdad de varianzas (Levene p > 0.05)  
- ✔ Diferencia significativa de medias (t-test p ≈ 0.0000)  

Conclusión:  
➡️ Los días lluviosos **prolongan de forma consistente** la duración de los viajes en esta ruta.

---

## 💡 Recomendaciones para Zuber

### ⭐ 1. Iniciar operaciones en zonas estratégicas  
Centrarse en Loop, River North y Streeterville para maximizar visibilidad y demanda.

### ⭐ 2. Gestionar flota según condiciones climáticas  
Aumentar disponibilidad o ajustar ETAs en días lluviosos para evitar retrasos.

### ⭐ 3. Integrar clima en el modelo de negocio  
Incorporar predicciones climáticas en la app para mejorar la experiencia del usuario.

---

## 🧰 Habilidades utilizadas
- Python (Pandas, NumPy, Seaborn, Matplotlib)  
- SQL  
- Visualización de datos  
- Análisis exploratorio (EDA)  
- Pruebas de hipótesis (Levene, t-test)  
- Limpieza y validación de datos  

---

## 🔗 Enlace al repositorio
https://github.com/utsa2004/proyectos-bootcamp-data-analyst-tripleten/tree/main/Proyecto%20Sprint%2008%20-%20Zuber

---


