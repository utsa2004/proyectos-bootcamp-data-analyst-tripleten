# 🧩 Proyecto 14.3 – Descomposición del Proyecto Final: CallMeMaybe  
**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción del proyecto

Este proyecto corresponde a la **fase de planeación analítica** del caso principal del proyecto final: **Telecomunicaciones – CallMeMaybe**.

Su objetivo es **descomponer el problema de negocio**, definir un **plan de análisis estructurado** y establecer los **criterios, métricas e hipótesis** que guiarán el desarrollo del análisis exploratorio y estadístico implementado posteriormente en el **Proyecto Final (14.4)**.

A diferencia de otros proyectos del portafolio, este notebook **no busca generar conclusiones finales**, sino sentar las bases metodológicas para un análisis sólido, reproducible y alineado a objetivos de negocio.

---

## 🎯 Objetivo del proyecto

Diseñar un **plan analítico estructurado** que permita:

- Comprender el problema operativo del cliente (CallMeMaybe).
- Definir qué se considera un **operador ineficaz** desde una perspectiva de datos.
- Establecer métricas, criterios y pruebas estadísticas apropiadas.
- Justificar el flujo de trabajo del análisis final.

---

## 🧠 Contexto del caso

CallMeMaybe es un servicio de telefonía virtual que busca identificar **operadores con bajo desempeño** dentro de sus clientes corporativos.

Un operador se considera potencialmente ineficaz si presenta:
- Alta cantidad de llamadas perdidas.
- Tiempos de espera prolongados.
- Bajo volumen de llamadas salientes.

Este proyecto aborda el **diagnóstico inicial del problema**, previo a cualquier modelado o validación estadística.

---

## 🧩 Estructura analítica definida

La descomposición del proyecto establece las siguientes etapas, que posteriormente se implementan en el análisis final:

1. Comprensión del contexto y objetivos de negocio.  
2. Preparación y revisión de los datasets.  
3. Exploración y limpieza de datos.  
4. Análisis exploratorio (EDA) y generación de métricas por operador.  
5. Definición de criterios de ineficiencia.  
6. Formulación y validación de hipótesis estadísticas.  
7. Síntesis de hallazgos y recomendaciones.  

> 📌 Nota: Los criterios utilizados se basan en distribuciones estadísticas y sirven como aproximación analítica. En un entorno real, estos umbrales deberían alinearse con KPIs definidos por el negocio.

---

## 📂 Dataset utilizados

- `telecom_dataset_us.csv` – Registro detallado de llamadas y eventos.
- `telecom_clients_us.csv` – Información de clientes y operadores.

---

## 🛠️ Herramientas y tecnologías

- Python
- pandas, numpy
- matplotlib, seaborn
- scipy (pruebas estadísticas)
- Pensamiento analítico estructurado

---

## 🔗 Relación con el Proyecto Final

Este proyecto **alimenta directamente** el desarrollo del:

👉 **Proyecto 14.4 – Proyecto Final CallMeMaybe**, donde el plan aquí definido se implementa mediante:
- Análisis exploratorio completo.
- Segmentación de operadores.
- Validación estadística de hipótesis.
- Identificación de ineficiencias operativas.

---

## 📂 Archivos del proyecto

- 📘 `Descomposicion_CallMeMaybe.ipynb` – Planeación y descomposición analítica
- 📄 `README.md` – Documentación del proyecto

---

## 🔗 Repositorio del proyecto

👉 *(aquí colocas el enlace al repositorio cuando lo pegues)*

---

## ✅ Estado del proyecto

✔ Descomposición analítica completada  
✔ Flujo de trabajo definido y justificado  
✔ Base metodológica establecida para el análisis final  

---

## 🧠 Nota final

Este proyecto demuestra la capacidad de **estructurar problemas complejos antes de analizarlos**, una habilidad clave en proyectos reales de analítica, donde definir correctamente el enfoque es tan importante como ejecutar el análisis.
