# 🧪 Proyecto Sprint 11 – A/B Testing y Priorización de Hipótesis (BigWeb)
## Evaluación de Experimentos para Incrementar Ingresos en una Tienda Online

**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción del proyecto
En este proyecto se realizó un análisis integral de un **experimento A/B** para la empresa ficticia **BigWeb**, una plataforma de comercio electrónico interesada en **incrementar sus ingresos** mediante cambios en la experiencia del usuario.

El análisis se dividió en dos grandes fases:

1. **Priorización de hipótesis de negocio** propuestas por el equipo de marketing.
2. **Evaluación estadística de un test A/B**, con el objetivo de determinar si el cambio aplicado al grupo experimental generó un impacto significativo en métricas clave como la **tasa de conversión** y el **ingreso promedio por pedido**.

---

## 🎯 Objetivo del proyecto
Ayudar a BigWeb a tomar **decisiones estratégicas basadas en datos**, utilizando frameworks de priorización y pruebas estadísticas para evaluar si una hipótesis de mejora debe implementarse, descartarse o seguir evaluándose.

---

## 📂 Conjuntos de datos utilizados

### 📁 Priorización de hipótesis
- **`hypotheses_us.csv`**
  - `Hypotheses`: descripción de la hipótesis
  - `Reach`: alcance del usuario (1–10)
  - `Impact`: impacto esperado (1–10)
  - `Confidence`: nivel de confianza (1–10)
  - `Effort`: esfuerzo requerido (1–10)

### 📁 Análisis del test A/B
- **`orders_us.csv`**
  - `transactionId`: identificador del pedido
  - `visitorId`: identificador del usuario
  - `date`: fecha del pedido
  - `revenue`: ingresos del pedido
  - `group`: grupo A/B

- **`visits_us.csv`**
  - `date`: fecha
  - `group`: grupo A/B
  - `visits`: número de visitas por día

---

## 🧩 Estructura del análisis

### 🔹 Paso 1: Priorización de hipótesis
Se evaluaron nueve hipótesis propuestas por el área de marketing utilizando dos frameworks:

- **ICE** (Impact, Confidence, Effort)
- **RICE** (Reach, Impact, Confidence, Effort)

Esto permitió comparar cómo cambia la priorización al incorporar el alcance de usuarios, justificando la selección de la hipótesis más prometedora.

---

### 🔹 Paso 2: Preparación de los datos
- Carga y exploración inicial de los datasets
- Conversión de tipos de datos (fechas y valores numéricos)
- Detección de usuarios presentes en ambos grupos
- Eliminación de duplicados y validación de consistencia

---

### 🔹 Paso 3: Análisis del test A/B
Se analizaron métricas clave para comparar los grupos A y B:

- Ingreso acumulado
- Tamaño promedio de pedido acumulado
- Diferencia relativa entre grupos
- Tasa de conversión diaria
- Distribución de pedidos por usuario
- Distribución de precios de pedidos

El análisis se realizó:
- Con **datos en bruto**
- Con **datos filtrados**, eliminando valores atípicos mediante percentiles 95 y 99

---

### 🔹 Paso 4: Pruebas estadísticas
Se aplicaron pruebas de significancia para evaluar diferencias entre los grupos:

- Prueba de Mann-Whitney U para:
  - Tasa de conversión
  - Tamaño promedio de pedido
- Evaluación con datos en bruto y datos filtrados
- Nivel de significancia definido explícitamente (α = 0.05)

---

## 📈 Resultados clave

- **Tasa de conversión**:
  - El grupo B mostró una mejora estadísticamente significativa frente al grupo A.
- **Ingreso promedio por pedido**:
  - No se identificaron diferencias estadísticamente significativas.
  - Al eliminar valores atípicos, el grupo B presentó un ingreso promedio ligeramente menor.
- **Impacto global**:
  - El aumento en conversión no se tradujo en un incremento significativo de ingresos totales.

---

## 🧾 Decisión final del experimento
🔴 **Se recomienda detener la prueba y no implementar la variante B**, ya que:

- Aunque la conversión mejoró,  
- No hubo evidencia estadística de un aumento en el ingreso promedio por pedido,  
- El impacto económico global no justifica la adopción del cambio.

---

## 💡 Recomendaciones adicionales
- Generar y evaluar nuevas hipótesis enfocadas directamente en **incrementar el ticket promedio**.
- Analizar segmentos específicos (usuarios nuevos vs recurrentes).
- Explorar combinaciones de estrategias que no solo aumenten la cantidad de usuarios que compran, sino también el monto promedio de cada    compra, por ejemplo mediante:
  - incentivos para que los usuarios elijan productos o planes de mayor valor, y
  - sugerencias de productos complementarios durante el proceso de compra.

---

## 🛠️ Herramientas y tecnologías utilizadas
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- SciPy (stats)  
- Análisis A/B  
- Estadística inferencial  

---

## 📂 Archivos del proyecto
📓 **Notebook principal**:  
- `Proyecto Sprint 11 - BigWeb.ipynb`

---

## ✅ Estado del proyecto
- ✔ Hipótesis priorizadas con ICE y RICE  
- ✔ Test A/B analizado estadísticamente  
- ✔ Decisión basada en evidencia

---

## 🔗 Enlace al repositorio
📎 https://github.com/utsa2004/proyectos-bootcamp-data-analyst-tripleten/tree/main/Proyecto%20Sprint11%20BigWeb

---

## 🧠 Nota final
Este proyecto demuestra la capacidad de **diseñar, analizar e interpretar experimentos A/B**, priorizar hipótesis de negocio y traducir resultados estadísticos en **decisiones estratégicas accionables**, fortaleciendo una cultura de toma de decisiones basada en datos.
