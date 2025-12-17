# 📡 Proyecto Sprint 5 – Megaline  
## Análisis Estadístico de Ingresos por Tarifas de Telecomunicaciones

**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción del proyecto
Megaline es un operador de telecomunicaciones que ofrece dos tarifas de prepago: **Surf** y **Ultimate**.  
El área comercial de la empresa busca determinar **cuál de estas tarifas genera mayores ingresos**, con el objetivo de optimizar su presupuesto de publicidad y sus estrategias comerciales.

En este proyecto se analizan datos de **500 clientes correspondientes al año 2018**, incluyendo información demográfica, consumo de llamadas, mensajes y datos móviles.

---

## 🎯 Objetivo del proyecto
Analizar el comportamiento de los clientes de Megaline y determinar, mediante **análisis estadístico**, qué tarifa de prepago genera mayores ingresos promedio, así como identificar diferencias de ingresos entre regiones.

---

## 📂 Datos utilizados
Se trabajó con múltiples conjuntos de datos que incluyen:

- Información de clientes y su plan tarifario
- Registro de llamadas (minutos)
- Registro de mensajes SMS
- Consumo de datos móviles
- Información regional de los usuarios

Los datos fueron agregados a nivel **mensual por usuario** para facilitar el análisis de ingresos.

---

### Conjuntos de datos utilizados
- `users.csv` – información de clientes y regiones
- `calls.csv` – registros de llamadas por usuario
- `messages.csv` – mensajes enviados
- `internet.csv` – consumo de datos móviles
- `plans.csv` – detalles de tarifas y precios

---

## 🧩 Etapas del análisis

### 🔹 Etapa 1: Exploración y preparación de datos
- Revisión de formatos y tipos de datos
- Conversión de fechas a formato `datetime`
- Identificación y tratamiento de valores ausentes
- Eliminación de duplicados
- Agrupación mensual de consumo por usuario

---

### 🔹 Etapa 2: Cálculo de ingresos
A partir del consumo mensual de cada cliente se calcularon los ingresos considerando:

- Cuota mensual del plan
- Minutos, mensajes y datos incluidos
- Consumo excedente y tarifas adicionales

El resultado fue un dataset consolidado con **ingresos mensuales por usuario**.

---

### 🔹 Etapa 3: Análisis exploratorio
- Comparación del consumo mensual entre planes
- Análisis de ingresos promedio por tarifa
- Cálculo de estadísticas descriptivas:
  - media
  - varianza
  - desviación estándar
- Visualización de distribuciones mediante histogramas y diagramas de caja

---

### 🔹 Etapa 4: Pruebas de hipótesis
Se plantearon y evaluaron dos hipótesis principales:

1. **Diferencia de ingresos entre tarifas Surf y Ultimate**
2. **Diferencia de ingresos entre la región NY/NJ y el resto de las regiones**

Para ambas hipótesis se aplicaron **pruebas t de Student**, utilizando un nivel de significancia del 5% (α = 0.05).

---

## 🛠️ Herramientas y tecnologías utilizadas
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **SciPy (stats)**
- Análisis estadístico inferencial
- Visualización de datos

---

## 📈 Resultados clave
- El ingreso promedio del plan **Ultimate** es mayor que el del plan **Surf**.
- La diferencia de ingresos entre planes es **estadísticamente significativa** (p < 0.05).
- Existen diferencias significativas de ingresos entre la región **NY/NJ** y el resto del país.
- Los usuarios fuera de NY/NJ presentan ingresos promedio y medianas más altas.
- Se observan patrones regionales que pueden influir en la estrategia comercial.

---

## 🧠 Conclusiones
Los resultados muestran evidencia estadística suficiente para concluir que:

- El plan **Ultimate** genera mayores ingresos promedio por usuario que el plan Surf.
- Existen diferencias regionales relevantes en los ingresos, siendo menores en el área de NY/NJ.
- Estas diferencias sugieren oportunidades para:
  - ajustar estrategias de marketing por región
  - diseñar campañas segmentadas
  - fomentar la adopción de planes más rentables

El análisis respalda la toma de decisiones comerciales basada en datos y evidencia estadística.

---

## 📂 Archivos del proyecto
- 📓 **Notebook principal:**  
  `notebook - Megaline.ipynb`

---

### ✅ Estado del proyecto
✔ Proyecto completado  
✔ Hipótesis evaluadas estadísticamente  

---

## 🔗 Enlace al repositorio
📎 https://github.com/utsa2004/proyectos-bootcamp-data-analyst-tripleten/tree/main/Proyecto%20Sprint%205%20-%20Megaline

---

## 🧠 Nota Final
Este proyecto demuestra experiencia en **análisis estadístico aplicado**, integración de datos de telecomunicaciones y traducción de resultados cuantitativos en **recomendaciones de negocio**.

