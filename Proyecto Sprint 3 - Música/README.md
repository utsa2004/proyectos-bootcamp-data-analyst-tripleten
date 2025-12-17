# 🎧 Proyecto Sprint 3 – Música  
## Análisis del Comportamiento de Escucha en Springfield y Shelbyville

**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción del proyecto
En este proyecto se analizan **datos reales de transmisión de música online** con el objetivo de comprender los hábitos de escucha de los usuarios en dos ciudades: **Springfield** y **Shelbyville**.

El análisis sigue el flujo completo de un proyecto de análisis de datos, que incluye la **descripción de los datos**, el **preprocesamiento**, la **prueba de una hipótesis** y la **interpretación de resultados**, permitiendo extraer conclusiones basadas en evidencia.

---

## 🎯 Objetivo del proyecto
Probar la hipótesis de que **la actividad de los usuarios al escuchar música varía según la ciudad y el día de la semana**, comparando el comportamiento de Springfield y Shelbyville.

---

## 📂 Datos utilizados
Los datos se encuentran en el archivo:

- `music_project_en.csv`

### Diccionario de datos
- **userID**: identificador único del usuario  
- **track**: nombre de la canción reproducida  
- **artist**: nombre del artista  
- **genre**: género musical  
- **city**: ciudad del usuario  
- **time**: hora de reproducción (HH:MM:SS)  
- **day**: día de la semana  

---

## 🧩 Etapas del análisis

### 🔹 Etapa 1: Descripción de los datos
- Exploración inicial de la estructura del dataset (`head`, `info`)
- Identificación de tipos de datos
- Detección de valores ausentes e inconsistencias

---

### 🔹 Etapa 2: Preprocesamiento de datos
- Corrección de nombres de columnas
- Identificación y tratamiento de valores ausentes
- Eliminación de duplicados
- Validación de la calidad de los datos antes del análisis

Estas acciones permitieron trabajar con un conjunto de datos más limpio y confiable.

---

### 🔹 Etapa 3: Análisis y prueba de la hipótesis
Se analizó el comportamiento de escucha:

- Comparando la cantidad de canciones reproducidas por ciudad
- Evaluando la actividad en días específicos de la semana (lunes, miércoles y viernes)
- Aplicando el enfoque **dividir – aplicar – combinar** mediante `groupby`

---

## 🛠️ Herramientas y tecnologías utilizadas
- **Python**
- **Pandas**
- Métodos de exploración (`head`, `info`)
- Limpieza de datos (`isna`, `dropna`, `drop_duplicates`)
- Agrupación y agregación (`groupby`, `count`)
- Análisis exploratorio de datos (EDA)

---

## 📈 Resultados y observaciones clave
- Springfield presenta un volumen de reproducciones significativamente mayor que Shelbyville.
- Al comparar por día de la semana, **miércoles** muestra menor actividad general.
- En Springfield, el día con más reproducciones es **viernes**.
- En Shelbyville, el patrón es distinto: **miércoles** presenta mayor actividad y **lunes** la menor.
- Los resultados sugieren diferencias claras en el comportamiento de escucha según ciudad y día.

---

## 🧠 Conclusiones
Los datos **respaldan la hipótesis planteada**:  
el comportamiento de los usuarios al escuchar música **varía según la ciudad y el día de la semana**.

Springfield y Shelbyville presentan patrones de consumo distintos, lo que indica que factores demográficos, sociales o de estilo de vida pueden influir en los hábitos de escucha.

> Nota: Este análisis es exploratorio. En proyectos reales, la validación de hipótesis suele complementarse con pruebas estadísticas formales.

---

## 📂 Archivos del proyecto
- 📓 **Notebook principal:**  
  `notebook - Música.ipynb`

---

### ✅ Estado del proyecto
✔ Proyecto completado  
✔ Hipótesis evaluada y documentada  

---

## 🔗 Enlace al repositorio
📎 https://github.com/utsa2004/proyectos-bootcamp-data-analyst-tripleten/tree/main/Proyecto%20Sprint%203%20-%20Música

---

## 🧠 Nota Final
Este proyecto demuestra la capacidad de realizar un **análisis exploratorio completo**, desde la limpieza de datos hasta la interpretación de resultados y conclusiones basadas en evidencia, utilizando herramientas estándar del análisis de datos.

