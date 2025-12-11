# Proyecto Sprint 10 – Showz: Análisis de Comportamiento de Usuarios y Rentabilidad de Marketing  
**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción del proyecto
Este proyecto analiza el comportamiento de los usuarios en **Showz**, una plataforma dedicada a la venta de entradas para eventos en línea. El objetivo es evaluar:

- El desempeño de las campañas de marketing  
- El valor que generan los usuarios a lo largo del tiempo  
- La rentabilidad de cada fuente de adquisición  
- Las oportunidades estratégicas para optimizar la inversión publicitaria  

Para ello se emplean tres datasets principales:

- **visits:** registros de visitas, sesiones y fuentes de tráfico  
- **orders:** historial de pedidos e ingresos por usuario  
- **costs:** inversión en marketing por fuente y fecha  

El análisis integra técnicas de limpieza de datos, métricas de negocio, cohortes, visualización, y cálculos de CAC, LTV y ROMI.

---

## 🎯 Objetivo del proyecto
Brindar recomendaciones estratégicas al equipo de marketing sobre:

- Dónde invertir  
- Cuánto invertir  
- Qué canales escalar o reducir  

Basado en la rentabilidad real de cada fuente, el valor del cliente y el comportamiento observado en la plataforma.

---

## 📂 Paso 1 – Preparación de los datos

Se realiza una exploración inicial de los datasets:

### ✔ Validaciones realizadas
- Identificación de valores nulos y duplicados  
- Conversión de datos a formatos adecuados (`datetime`, numéricos, categóricos)  
- Verificación de consistencia entre fechas y registros  
- Revisión de unicidad e integridad por usuario y fuente  

### ✔ Variables clave analizadas
- Duración de sesiones  
- Frecuencia de visitas  
- Fechas de conversión  
- Ingresos generados por usuario  
- Costo de adquisición por campaña  

Esta base garantiza un análisis sólido y libre de errores estructurales.

---

## 📈 Paso 2 – Métricas clave del negocio

Durante esta fase se analizan tres áreas principales:

---

### 🔹 **1. Comportamiento de visitas**
- Volumen de usuarios diarios  
- Sesiones promedio por usuario  
- Diferencias entre dispositivos  
- Desempeño por fuente de tráfico  

### 🔹 **2. Dinámica de ventas**
- Momento en que los usuarios compran  
- Número de pedidos por usuario  
- Cálculo del **LTV (Lifetime Value)**  
- Análisis de cohortes por fecha de adquisición  

### 🔹 **3. Rendimiento del marketing**
Se calculan:

| Métrica | Descripción |
|--------|-------------|
| **CAC** | Costo de adquirir un nuevo cliente |
| **LTV** | Valor de ingresos generado por cliente |
| **ROMI** | Retorno de la inversión en marketing |
| Tiempo hasta la conversión | Días entre primera visita y primera compra |

Además se generan visualizaciones que muestran:

- Eficiencia comparada entre fuentes  
- Evolución del gasto vs. ingresos  
- Distribución de clientes por canal  
- Relación entre dispositivos y conversión  

---

## 🧠 Paso 3 – Conclusiones estratégicas

### 🔝 **Fuentes más rentables:** 1, 2 y 5  
Estas fuentes destacan porque:

- Tienen los mejores ROMI:
  - Fuente 1 → **ROMI: 110.31**  
  - Fuente 2 → **ROMI: 61.63**  
  - Fuente 5 → **ROMI: 22.83**
- Presentan un balance sólido entre **LTV alto y CAC medio-bajo**  
- Generan conversiones rápidas y comportamiento recurrente  

📌 **Recomendación:**  
Destinar **60–70% del presupuesto total** a estas fuentes, dando mayor prioridad a la fuente 1 por su excepcional retorno.

---

### ⚠️ **Fuentes que requieren ajustes:** 3 y 10

#### **Fuente 3**  
- Acapara **43% del presupuesto total**  
- Tiene un **ROMI muy bajo: 2.10**  
- Presenta el CAC más alto (10.21)

➡️ **Recomendación:** Optimizar segmentación o pausar temporalmente si no mejora.

#### **Fuente 10**  
- ROMI bajo (**2.51**)  
- Bajo volumen de compradores  
- CAC bajo, pero ingresos insuficientes

➡️ **Recomendación:** Mantener solo como canal experimental <5%.

---

### 🧪 **Fuente con potencial de crecimiento:** 9

- CAC más bajo del conjunto (**1.98**)  
- ROMI aún moderado (**6.59**)  
- Comportamiento prometedor

➡️ **Recomendación:** Incremento gradual de presupuesto.

---

## 📊 Métricas clave utilizadas
- **CAC:** eficiencia económica por cliente adquirido  
- **LTV:** valor promedio generado por usuario  
- **ROMI:** retorno real del gasto publicitario  
- **Análisis de comportamiento:** tamaño de compra, recurrencia, velocidad de conversión  

---

## 🧩 Conclusión final
El análisis muestra que Showz ya posee canales de marketing altamente rentables que deben escalarse, mientras que otros requieren una revisión profunda o reducción de inversión.  
Aplicar esta redistribución optimizada permitirá:

- Mejorar el retorno financiero del marketing  
- Aumentar la adquisición eficiente de usuarios  
- Construir una base de clientes rentable y sostenible  
- Tomar decisiones estratégicas basadas en datos reales  

---

## 🧰 Habilidades utilizadas
- Python (Pandas, NumPy, Matplotlib, Seaborn)  
- ETL básico  
- Análisis de cohortes  
- Métricas de negocio (CAC, LTV, ROMI)  
- Visualización de datos  
- Evaluación de rentabilidad  
- Storytelling analítico  

---

## 🔗 Enlace al repositorio
https://github.com/utsa2004/proyectos-bootcamp-data-analyst-tripleten/tree/main/Proyecto%20Sprint%2010%20-%20Showz

---

