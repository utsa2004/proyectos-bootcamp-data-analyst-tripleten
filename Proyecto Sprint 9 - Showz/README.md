# 🎟️ Proyecto Sprint 9 – Showz  
## Análisis de Negocio y Marketing para Plataforma de Venta de Entradas

**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción del proyecto
Showz es una plataforma dedicada a la venta de entradas para eventos en línea.  
El equipo de marketing busca entender el comportamiento de los usuarios desde su primera visita hasta la compra, así como evaluar la efectividad de las campañas publicitarias y el valor que generan los clientes a lo largo del tiempo.

En este proyecto se realiza un **análisis integral de negocio**, combinando datos de visitas, pedidos y costos de marketing para medir métricas clave como **CAC, LTV y ROMI**, y generar recomendaciones estratégicas basadas en datos reales.

---

## 🎯 Objetivo del proyecto
Evaluar el desempeño de las campañas de marketing de Showz para:

- Identificar los canales de adquisición más rentables  
- Optimizar la distribución del presupuesto publicitario  
- Maximizar el retorno sobre la inversión en marketing (ROMI)  
- Comprender el comportamiento de los usuarios a lo largo del tiempo  

---

## 📂 Conjuntos de datos utilizados
Se trabajó con tres fuentes principales de datos:

- **visits**: registros de visitas a la plataforma (inicio y fin de sesión, dispositivo, fuente de tráfico)
- **orders**: historial de pedidos realizados por los usuarios (fecha de compra e ingresos)
- **costs**: gastos de marketing por fuente de adquisición y fecha

Estos datasets permitieron analizar el recorrido completo del usuario, desde la adquisición hasta la generación de ingresos.

---

## 🧩 Estructura del análisis

### 🔹 Paso 1: Preparación de los datos
- Carga y exploración inicial de los datasets
- Revisión de valores nulos y duplicados
- Verificación y corrección de tipos de datos (fechas, valores numéricos)
- Transformaciones necesarias para el análisis de métricas de negocio

---

### 🔹 Paso 2: Informes y métricas clave
El análisis se centró en tres dimensiones principales:

#### 📈 Visitas
- Número de usuarios
- Frecuencia de visitas
- Duración de sesiones
- Comportamiento por dispositivo y fuente de tráfico

#### 💰 Ventas
- Número de pedidos
- Ingresos generados
- Valor de vida del cliente (LTV)
- Comportamiento de compra a lo largo del tiempo

#### 📣 Marketing
- Costo de adquisición de clientes (CAC)
- Retorno sobre la inversión en marketing (ROMI)
- Comparación de desempeño entre fuentes de adquisición

Se utilizaron visualizaciones para analizar tendencias, comparar fuentes y evaluar la evolución de las métricas clave.

---

## 🧪 Métricas utilizadas
Las decisiones de negocio se basaron principalmente en:

- **CAC (Customer Acquisition Cost)**: costo promedio para adquirir un cliente
- **LTV (Lifetime Value)**: ingreso promedio generado por cliente
- **ROMI (Return on Marketing Investment)**: rentabilidad real de cada fuente de marketing
- Métricas de comportamiento: tiempo hasta la conversión y tamaño promedio de compra

---

## 📊 Resultados clave

### 🔝 Fuentes recomendadas: 1, 2 y 5
Estas fuentes destacan como las más eficientes y rentables:

- **Fuente 1**: ROMI ≈ 110.31  
- **Fuente 2**: ROMI ≈ 61.63  
- **Fuente 5**: ROMI ≈ 22.83  

Presentan:
- Alto retorno por dólar invertido
- Buen equilibrio entre LTV y CAC
- Comportamiento positivo en conversión y recurrencia

---

### ⚠️ Fuentes a revisar: 3 y 10
- **Fuente 3**:
  - Alta inversión (~43% del presupuesto)
  - ROMI bajo (≈ 2.10)
  - CAC más alto del conjunto  
  - Recomendación: optimizar campañas o suspender temporalmente

- **Fuente 10**:
  - ROMI bajo (≈ 2.51)
  - Bajo volumen de compradores  
  - Recomendación: mantener inversión mínima (<5%) como canal experimental

---

### 🧪 Fuente con potencial de crecimiento: 9
- CAC más bajo del análisis (≈ 1.98)
- ROMI moderado (≈ 6.59)
- Recomendación: aumentar gradualmente la inversión y evaluar su escalabilidad

---

## 🧠 Conclusiones y recomendaciones
El análisis demuestra que Showz cuenta con canales altamente rentables que deben ser priorizados, mientras que otros requieren ajustes o reducción de inversión.

**Recomendación principal:**
- Redistribuir el presupuesto de marketing asignando **60%–70%** a las fuentes **1, 2 y 5**, con mayor peso en la fuente 1 debido a su alto retorno.

Esta estrategia permitiría:
- Mejorar el rendimiento financiero del marketing
- Atraer clientes más valiosos
- Construir una base de usuarios más rentable y sostenible a largo plazo

---

## 🛠️ Herramientas y tecnologías utilizadas
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Análisis de métricas de negocio  
- Visualización de datos  

---

## 📂 Archivos del proyecto
📓 **Notebook principal**:  
- `notebook - Showz.ipynb`

---

## ✅ Estado del proyecto
- ✔ Proyecto completado  
- ✔ Métricas de negocio analizadas  
- ✔ Recomendaciones estratégicas documentadas  

---

## 🔗 Enlace al repositorio
📎 https://github.com/utsa2004/proyectos-bootcamp-data-analyst-tripleten/tree/main/Proyecto%20Sprint%2010%20-%20Showz

---

## 🧠 Nota final
Este proyecto demuestra la capacidad de realizar un análisis de negocio orientado a marketing, integrando datos de usuarios, ventas y costos para generar recomendaciones estratégicas basadas en métricas clave como CAC, LTV y ROMI.
