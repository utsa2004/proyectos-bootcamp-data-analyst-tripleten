# 🏋️ Proyecto Sprint 14 – Análisis de Retención de Clientes en Model Fitness  
**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción del proyecto

En este proyecto se realizó un **análisis integral de retención de clientes (churn)** para *Model Fitness*, una cadena de gimnasios que busca reducir la cancelación de membresías mediante el uso de **análisis de datos y aprendizaje automático**.

El estudio combina análisis exploratorio, modelos predictivos supervisados y técnicas de segmentación no supervisadas para **identificar patrones de abandono**, comprender el comportamiento de los clientes y proponer **estrategias accionables de retención** basadas en datos.

---

## 🎯 Objetivo del proyecto

Dotar a Model Fitness de una solución analítica que permita:

- Predecir la **probabilidad de cancelación** de clientes para el mes siguiente.
- Identificar los **factores más influyentes** en el abandono.
- Construir **perfiles de clientes** mediante segmentación.
- Formular **recomendaciones estratégicas** para reducir la rotación y aumentar la lealtad.

---

## 📂 Conjunto de datos utilizado

**Archivo:** `gym_churn_us.csv`

El dataset contiene información histórica de clientes, incluyendo:

### 🔹 Variable objetivo
- `Churn`: indica si el cliente canceló su membresía en el mes analizado.

### 🔹 Características del cliente
- `gender`
- `Near_Location`
- `Partner`
- `Promo_friends`
- `Phone`
- `Age`
- `Lifetime` (meses desde la primera inscripción)

### 🔹 Uso del servicio y contrato
- `Contract_period`
- `Month_to_end_contract`
- `Group_visits`
- `Avg_class_frequency_total`
- `Avg_class_frequency_current_month`
- `Avg_additional_charges_total`

---

## 🔍 Metodología de análisis

### 📊 1. Análisis exploratorio de datos (EDA)
- Revisión de valores nulos y estadísticos descriptivos.
- Comparación de características entre clientes que cancelaron y los que permanecieron.
- Visualización de distribuciones e histogramas.
- Análisis de correlación entre variables.

### 🤖 2. Modelos predictivos supervisados
Se entrenaron y evaluaron dos modelos de clasificación binaria:
- **Regresión Logística**
- **Random Forest**

Los modelos fueron evaluados utilizando:
- Accuracy
- Precision
- Recall

📌 La **Regresión Logística** mostró el mejor equilibrio entre métricas, destacando especialmente en la detección de clientes en riesgo.

### 🧩 3. Segmentación de clientes (Clustering)
- Estandarización de variables.
- Análisis jerárquico y dendrograma.
- Clustering con **K-Means (k = 5)**.
- Evaluación de clústeres mediante medias de características y tasa de cancelación.

---

## 📈 Resultados clave

### 🔹 Predicción de cancelación
- El modelo de Regresión Logística alcanzó una **precisión del 92 %** y un **recall del 82.8 %**.
- Las variables más influyentes en la cancelación fueron:
  - Frecuencia de asistencia.
  - Antigüedad del cliente.
  - Duración del contrato.

### 🔹 Segmentación de clientes
- Se identificaron **5 clústeres** con comportamientos diferenciados.
- Dos clústeres presentaron **altas tasas de cancelación** (≈44 % y ≈51 %), asociados a:
  - Baja frecuencia de uso.
  - Menor antigüedad.
- Otros clústeres mostraron alta fidelidad y compromiso.

---

## 💡 Recomendaciones estratégicas

1. 🔔 **Alertas tempranas de riesgo**  
   Utilizar el modelo predictivo para identificar semanalmente a clientes con alta probabilidad de abandono.

2. 🎁 **Programas de fidelización personalizados**  
   Reforzar beneficios para clientes leales y activos (descuentos por antigüedad, recompensas).

3. 📆 **Incentivar contratos de mayor duración**  
   Promover planes de 6–12 meses con incentivos por permanencia.

4. 💬 **Fomentar comunidad y participación**  
   Clases grupales, desafíos mensuales y dinámicas sociales para clientes con baja actividad.

5. 📊 **Monitoreo continuo de métricas clave**
   - Tasa mensual de cancelación.
   - Frecuencia promedio de uso.
   - Evolución de clientes en riesgo.

---

## 🛠️ Herramientas y tecnologías utilizadas

- Python
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- Modelos supervisados y no supervisados
- Análisis exploratorio y estadístico

---

## 📂 Archivos del proyecto

- 📘 `gym_churn_us.csv` – Dataset utilizado
- 📓 `Proyecto_Sprint_14_Model_Fitness.ipynb` – Notebook de análisis
- 📄 `README.md` – Documentación del proyecto

---

## ✅ Estado del proyecto

✔ Análisis exploratorio completado  
✔ Modelos predictivos entrenados y evaluados  
✔ Segmentación de clientes realizada  
✔ Recomendaciones estratégicas definidas  

---

## 🔗 Repositorio del proyecto

👉 *(https://github.com/utsa2004/proyectos-bootcamp-data-analyst-tripleten/tree/main/Proyecto%20Sprint%2014%20-%20Fitness)*

---

## 🧠 Nota final

Este proyecto demuestra cómo el **análisis de datos y el aprendizaje automático** pueden aplicarse directamente a problemas reales de negocio, permitiendo anticipar la pérdida de clientes y diseñar **estrategias de retención basadas en evidencia**, orientadas a mejorar la experiencia del usuario y la rentabilidad a largo plazo.

