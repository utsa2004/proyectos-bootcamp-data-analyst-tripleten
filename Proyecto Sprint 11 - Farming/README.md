# 🥗 Proyecto Sprint 11 – Farming  
## Análisis de Embudo de Conversión y Test A/A/B en una App de Productos Alimenticios

**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción del proyecto
Farming es una empresa emergente dedicada a la venta de productos alimenticios a través de una aplicación móvil.  
El equipo de producto busca comprender el comportamiento de los usuarios dentro de la app, identificar **cuellos de botella en el proceso de compra** y evaluar si un **cambio visual en la interfaz (fuentes tipográficas)** afecta la interacción de los usuarios.

Para ello, se realiza un análisis integral que combina:
- estudio del **embudo de conversión**, y  
- evaluación de un **experimento A/A/B** para validar cambios de diseño de forma estadísticamente confiable.

---

## 🎯 Objetivo del proyecto
- Analizar cómo los usuarios avanzan a lo largo del embudo de compra.
- Identificar las etapas donde se pierden más usuarios.
- Evaluar si el rediseño tipográfico tiene un impacto significativo en el comportamiento del usuario.
- Garantizar la validez estadística del experimento mediante un test A/A/B.

---

## 📂 Conjunto de datos utilizado
Se trabajó con un único dataset que registra eventos de usuario:

- **logs_exp_us.csv** – registro de eventos de la aplicación

### Descripción de las variables
- **EventName**: nombre del evento (pantalla o acción del usuario)
- **DeviceIDHash**: identificador único del usuario
- **EventTimestamp**: fecha y hora del evento
- **ExpId**: grupo experimental  
  - 246 y 247 → grupos de control  
  - 248 → grupo de prueba (nueva fuente)

Cada fila representa una acción realizada por un usuario dentro de la aplicación.

---

## 🧩 Etapas del análisis

### 🔹 Etapa 1: Preparación de los datos
- Renombrado de columnas para facilitar el análisis
- Conversión de tipos de datos (fechas y horas)
- Eliminación de duplicados
- Verificación de valores nulos
- Creación de columnas de fecha y hora separadas
- Validación de usuarios únicos por grupo experimental

---

### 🔹 Etapa 2: Exploración general de los datos
- Número total de eventos y usuarios
- Promedio de eventos por usuario
- Análisis del periodo de tiempo cubierto
- Identificación del rango temporal con datos completos
- Verificación de la distribución equilibrada entre los tres grupos experimentales

---

### 🔹 Etapa 3: Análisis del embudo de conversión
- Identificación de eventos y su frecuencia
- Cálculo del número y proporción de usuarios por evento
- Construcción del embudo secuencial
- Cálculo de conversiones entre etapas
- Identificación de la etapa con mayor abandono
- Estimación del porcentaje de usuarios que completan todo el recorrido hasta el pago

---

### 🔹 Etapa 4: Evaluación del experimento A/A/B
- Comparación entre los dos grupos de control (A/A) para validar la correcta aleatorización
- Análisis de eventos clave por grupo
- Pruebas de hipótesis para comparar proporciones de usuarios entre grupos
- Comparación del grupo experimental frente a:
  - cada grupo de control por separado
  - los grupos de control combinados
- Ajuste del nivel de significancia considerando múltiples pruebas (Bonferroni)

---

## 🛠️ Herramientas y tecnologías utilizadas
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Plotly Express  
- SciPy  
- Statsmodels (pruebas de proporciones)  
- Análisis de embudos  
- Pruebas estadísticas A/A/B  

---

## 📈 Resultados clave

### 🔍 Embudo de conversión
- Conversión total del embudo ≈ **47%**
- Mayor fuga de usuarios entre **MainScreen → OffersScreen** (≈40%)
- Alta probabilidad de pago una vez que el usuario llega al carrito (≈95%)

### 🧪 Experimento A/A/B
- Distribución equilibrada de usuarios entre grupos (≈2,500 por grupo)
- Los grupos de control no presentan diferencias estadísticamente significativas
- El cambio de fuentes **no genera impacto significativo** en ningún evento
- Resultados robustos incluso tras aplicar correcciones por múltiples pruebas

---

## 🧠 Conclusiones y recomendaciones
- El experimento A/A/B confirma que el rediseño tipográfico es **neutral** en términos de impacto sobre el comportamiento del usuario.
- El principal cuello de botella del proceso de compra se encuentra en la transición **Main → Offers**.
- Se recomienda enfocar esfuerzos de optimización en esta etapa mediante:
  - mejoras visuales,
  - mensajes de incentivo,
  - optimización del rendimiento y tiempos de carga.

El análisis proporciona una base sólida y confiable para priorizar mejoras que aumenten la conversión sin introducir riesgos innecesarios.

---

## 📂 Archivos del proyecto
📓 **Notebook principal**:  
- `notebook - Farming.ipynb`

---

## ✅ Estado del proyecto
- ✔ Proyecto completado  
- ✔ Embudo de conversión analizado  
- ✔ Experimento A/A/B validado estadísticamente  

---

## 🔗 Enlace al repositorio
📎 https://github.com/utsa2004/proyectos-bootcamp-data-analyst-tripleten/tree/main/Proyecto%20Sprint%2012%20-%20Farming

---

## 🧠 Nota final
Este proyecto demuestra la capacidad de analizar el comportamiento de usuarios, construir embudos de conversión, diseñar y validar experimentos A/A/B y traducir resultados estadísticos en recomendaciones prácticas para producto y experiencia de usuario.

