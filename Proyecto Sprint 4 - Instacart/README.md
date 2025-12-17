# 🛒 Proyecto Sprint 4 – Instacart  
## Análisis Exploratorio de Hábitos de Compra en una Plataforma de E-commerce

**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción del proyecto
En este proyecto se analizan datos reales de **Instacart**, una plataforma de entrega de comestibles similar a Uber Eats o DoorDash.  
El conjunto de datos fue publicado originalmente para una competencia de Kaggle y posteriormente modificado para incluir **valores ausentes y duplicados**, conservando las distribuciones originales.

El objetivo principal es **limpiar, procesar y analizar los datos** para obtener información relevante sobre los **hábitos de compra y recompra de los clientes**, así como patrones temporales y de comportamiento de consumo.

---

## 🎯 Objetivo del proyecto
Limpiar y preparar múltiples tablas de datos relacionales y realizar un **análisis exploratorio** que permita identificar patrones de compra, recompra y comportamiento temporal de los clientes de Instacart.

---

## 📂 Conjunto de datos utilizado
Se trabajó con cinco tablas principales:

- **instacart_orders.csv** – información de pedidos  
- **products.csv** – información de productos  
- **order_products.csv** – productos incluidos en cada pedido  
- **aisles.csv** – pasillos de supermercado  
- **departments.csv** – departamentos de productos  

Estas tablas se integran para permitir un análisis completo del comportamiento de compra.

---

## 🧩 Etapas del análisis

### 🔹 Etapa 1: Descripción de los datos
- Lectura de archivos CSV con formato no estándar (`sep=';'`)
- Exploración inicial con `head()` e `info()`
- Uso de `info(show_counts=True)` para DataFrames con un gran volumen de filas
- Identificación de valores ausentes, duplicados y tipos de datos inconsistentes

---

### 🔹 Etapa 2: Preprocesamiento de los datos
- Corrección de tipos de datos en columnas numéricas
- Tratamiento diferenciado de valores ausentes:
  - Identificación de valores NaN con significado lógico (primer pedido)
  - Relleno controlado de valores ausentes en nombres de productos
  
- Eliminación de duplicados explícitos
- Validación de duplicados implícitos sin impacto analítico
- Normalización de nombres de productos

---

### 🔹 Etapa 3: Análisis exploratorio (EDA)
Se analizaron, entre otros aspectos:

- Distribución de pedidos por hora del día
- Distribución de pedidos por día de la semana
- Tiempo entre pedidos consecutivos
- Diferencias en comportamiento entre días específicos
- Número de productos por pedido
- Productos más pedidos y más reordenados
- Proporción de recompra por producto y por cliente
- Productos que se agregan primero al carrito

Se utilizaron gráficos para comunicar claramente los resultados.

---

## 🛠️ Herramientas y tecnologías utilizadas
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- Técnicas de limpieza de datos
- Análisis exploratorio de datos (EDA)
- Visualización de datos

---

## 📈 Resultados y hallazgos clave
- La mayoría de los pedidos contienen **pocos artículos**, con una media cercana a 10 productos.
- El mayor volumen de compras ocurre **entre domingo y lunes**.
- La actividad de compra es mayor **entre las 10 a.m. y las 4 p.m.**
- Los productos más populares son **alimentos frescos** como frutas y vegetales.
- Muchos de los productos más reordenados son artículos de consumo frecuente.
- Existe una alta variabilidad en la tasa de recompra entre productos y clientes.
- Los productos más vendidos suelen ser de **bajo margen**, lo que sugiere oportunidades estratégicas.

---

## 🧠 Conclusiones
El análisis muestra que el modelo de negocio de Instacart se basa en **alto volumen y baja unidad de margen**, con una fuerte dependencia de productos de consumo recurrente.

Se identifican oportunidades claras para:
- Incrementar el valor promedio del pedido
- Promover productos de mayor margen
- Fomentar la recompra en periodos posteriores al inicio del mes
- Diseñar estrategias de fidelización basadas en patrones de consumo

---

## 📂 Archivos del proyecto
- 📓 **Notebook principal:**  
  `notebook - Instacart.ipynb`

---

### ✅ Estado del proyecto
✔ Proyecto completado  
✔ Análisis exploratorio documentado  

---

## 🔗 Enlace al repositorio
📎 https://github.com/utsa2004/proyectos-bootcamp-data-analyst-tripleten/tree/main/Proyecto%20Sprint%204%20-%20Instacart

---

## 🧠 Nota para reclutadores
Este proyecto demuestra experiencia en **limpieza de datos complejos**, integración de múltiples tablas y análisis exploratorio orientado a negocio en un entorno real de e-commerce.

