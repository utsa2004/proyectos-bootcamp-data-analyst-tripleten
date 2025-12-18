# 🧪 14.1 Proyecto – Pruebas A/B  
**Sprint 14 – Proyecto Final**  
**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción del proyecto

Una empresa internacional de comercio electrónico lanzó una **prueba A/B** con el objetivo de evaluar el impacto de un **nuevo sistema de recomendaciones de productos** sobre el comportamiento de los usuarios dentro del embudo de conversión.

El experimento, denominado **`recommender_system_test`**, compara:

- **Grupo A (control):** embudo de pago actual  
- **Grupo B (experimental):** embudo con sistema de recomendaciones mejorado  

El análisis se centra en usuarios **nuevos de la región de la UE**, evaluando si el nuevo sistema logra mejorar las tasas de conversión en las principales etapas del embudo de compra.

---

## 🎯 Objetivo del estudio

### 🔸 Objetivo principal
Determinar si la introducción del nuevo sistema de recomendaciones genera una **mejora estadísticamente significativa (≥10%)** en las tasas de conversión del embudo de compras.

### 🔹 Objetivos específicos
Evaluar el impacto del sistema mejorado en las siguientes etapas del embudo:

- `product_page` – vistas de página de producto  
- `product_cart` – productos añadidos al carrito  
- `purchase` – compras realizadas  

Asimismo, se busca **validar la correcta ejecución del experimento**, analizar la consistencia de los datos y evaluar los resultados mediante una **prueba Z para diferencias de proporciones**.

---

## 🧪 Especificaciones técnicas del experimento

- **Nombre de la prueba:** `recommender_system_test`
- **Periodo del experimento:**  
  - Inicio: 07-12-2020  
  - Fin: 01-01-2021  
- **Cierre de registro de nuevos usuarios:** 21-12-2020
- **Audiencia:** 15% de los nuevos usuarios de la región UE
- **Participantes esperados:** ~6,000 usuarios
- **Resultado esperado:**  
  Incremento ≥10% en cada etapa del embudo  
  `product_page → product_cart → purchase`  
  dentro de los primeros 14 días tras el registro

---

## 📂 Conjuntos de datos utilizados

Se trabajó con cuatro datasets proporcionados por la plataforma:

- **`ab_project_marketing_events_us.csv`**  
  Calendario de eventos de marketing activos durante el experimento.

- **`final_ab_new_users_upd_us.csv`**  
  Información de usuarios nuevos registrados durante el periodo de prueba.

- **`final_ab_events_upd_us.csv`**  
  Registro de eventos de comportamiento de los usuarios (vistas, carrito, compras).

- **`final_ab_participants_upd_us.csv`**  
  Asignación de usuarios a los grupos A y B del experimento.

Estos datasets permiten analizar tanto la **consistencia del experimento** como el **comportamiento completo del usuario dentro del embudo**.

---

## 🔍 Metodología de análisis

El proyecto se desarrolló en dos etapas principales:

### 1️⃣ Análisis exploratorio de datos (EDA)
- Validación de tipos de datos, valores ausentes y duplicados
- Verificación de equilibrio entre grupos
- Análisis de eventos por usuario
- Distribución temporal de eventos
- Detección de posibles anomalías o sesgos
- Evaluación de la coherencia del embudo de conversión

### 2️⃣ Evaluación estadística de la prueba A/B
- Cálculo de tasas de conversión por etapa
- Comparación entre grupos A y B
- Aplicación de **prueba Z para diferencias de proporciones**
- Interpretación de resultados bajo un nivel de significancia α = 0.05

---

## 🛠️ Herramientas y tecnologías utilizadas

- Python  
- Pandas y NumPy  
- Matplotlib y Seaborn  
- Plotly Express  
- `statsmodels` (prueba Z de proporciones)  

---

## 📊 Resultados clave

- El análisis exploratorio confirmó:
  - Equilibrio adecuado entre grupos
  - Ausencia de usuarios duplicados entre muestras
  - Distribución homogénea de eventos en el tiempo
  - Correcta ejecución técnica del experimento

- Los resultados de la prueba A/B mostraron que:
  - El **grupo B no superó al grupo A** en ninguna etapa del embudo
  - Las diferencias observadas en conversión **no fueron estadísticamente significativas**  
    (p-valor > 0.05 en todos los casos)

---

## 🧠 Conclusiones y recomendaciones

El nuevo sistema de recomendaciones **no cumplió el objetivo del experimento**, ya que no logró incrementar las tasas de conversión en al menos un 10% en ninguna de las etapas del embudo.

Desde una perspectiva de negocio, se concluye que **no es recomendable implementar el sistema en su estado actual**.

### Recomendaciones:
- Revisar la calidad y relevancia de las recomendaciones generadas
- Analizar segmentos específicos de usuarios para detectar efectos ocultos
- Diseñar una nueva prueba A/B con ajustes en el algoritmo o en la muestra
- Complementar el sistema de recomendaciones con mejoras en UX o contenido

---

## 📂 Archivos del proyecto

- 📓 `notebook Proyecto AB Test.ipynb`
- 📘 `README.md`

---

## ✅ Estado del proyecto

✔ Análisis exploratorio completo  
✔ Evaluación estadística documentada  
✔ Conclusiones alineadas a objetivos de negocio  

---

## 🧭 Nota final

Este proyecto demuestra la importancia de **validar hipótesis de negocio mediante análisis estadístico riguroso**. Aunque el experimento no validó la mejora esperada, el proceso analítico permitió obtener información valiosa sobre el comportamiento del usuario y sentar bases sólidas para futuras iteraciones del sistema de recomendaciones.

