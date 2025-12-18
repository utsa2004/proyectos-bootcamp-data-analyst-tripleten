# 📡 Proyecto 14.4 – Telecomunicaciones: Identificación de Operadores Ineficaces (CallMeMaybe)
**Bootcamp de Data Analytics – TripleTen**  

---

## 📷 Vista previa del dashboard

<img width="979" height="479" alt="dashboard_callmemaybe_operadores" src="https://github.com/user-attachments/assets/28d0bfcb-f42c-441e-a8c6-430234005207" />

📊 **Dashboard interactivo de eficiencia operativa**, donde se visualizan métricas clave del desempeño de los operadores de CallMeMaybe, incluyendo duración de llamadas, participación de llamadas internas y externas, volumen diario de actividad y filtros dinámicos por tipo y dirección de llamada.  

Este dashboard complementa el análisis estadístico del proyecto y permite a supervisores identificar patrones de ineficiencia de forma visual e intuitiva.

---

## 📌 Descripción del proyecto

Este proyecto corresponde al **caso principal del Proyecto Final** y tiene como objetivo analizar el desempeño operativo de los operadores del servicio de telefonía virtual **CallMeMaybe**, con el fin de **identificar operadores ineficaces y validar estadísticamente dichas ineficiencias**.

El análisis integra **exploración de datos, métricas operativas, pruebas de hipótesis estadísticas y visualización**, permitiendo transformar datos de alto volumen en información accionable para supervisores y tomadores de decisión.

Este notebook implementa el plan analítico definido previamente en el **Proyecto 14.3 – Descomposición del Proyecto Final**.

---

## 🎯 Objetivo del proyecto

Detectar operadores con bajo desempeño operativo mediante:

- Análisis exploratorio de datos (EDA).
- Definición de métricas de eficiencia.
- Identificación de operadores ineficaces.
- Validación estadística de las diferencias observadas.

---

## 🧠 Criterios de ineficiencia operativa

Un operador se considera potencialmente **ineficaz** si presenta uno o más de los siguientes patrones:

- Alta cantidad de llamadas entrantes perdidas (internas y externas).
- Tiempos de espera prolongados en llamadas entrantes externas.
- Bajo volumen de llamadas salientes externas (cuando aplica).

> 📌 Nota: Los umbrales utilizados se basan en la distribución estadística de los datos. En un entorno real, estos criterios deberían alinearse con KPIs operativos definidos por el negocio.

---

## 🧩 Hipótesis estadísticas evaluadas

**Hipótesis 1 – Llamadas entrantes perdidas**  
- H₀: No existen diferencias significativas entre operadores.  
- H₁: Existen diferencias significativas entre operadores.

**Hipótesis 2 – Tiempo de espera en llamadas entrantes externas**  
- H₀: No existen diferencias significativas entre operadores.  
- H₁: Existen diferencias significativas entre operadores.

**Hipótesis 3 – Llamadas salientes externas**  
- H₀: No existen diferencias significativas entre operadores.  
- H₁: Existen diferencias significativas entre operadores.

Las hipótesis fueron evaluadas mediante **test de Levene** y **pruebas t de Student**, seleccionando el enfoque adecuado según la homogeneidad de varianzas.

---

## 📂 Datasets utilizados

- **`telecom_dataset_us.csv`**  
  Registros detallados de llamadas: dirección, tipo, duración, llamadas perdidas y métricas de espera.

- **`telecom_clients_us.csv`**  
  Información de clientes corporativos: plan tarifario y fecha de inicio.

---

## 🛠️ Herramientas y tecnologías

- Python  
- pandas, numpy  
- matplotlib, seaborn  
- scipy (estadística inferencial)  
- Tableau Public (dashboard interactivo)

---

## 📈 Principales hallazgos

- Se identificó un grupo de **25 operadores con bajo desempeño**, mostrando patrones consistentes de ineficiencia.
- Los operadores ineficaces presentan:
  - Mayor volumen de llamadas perdidas.
  - Tiempos de espera significativamente más altos.
  - Menor actividad saliente.
- Las pruebas estadísticas confirmaron que estas diferencias **son significativas y no atribuibles al azar** (p < 0.05).

---

## 📊 Dashboard interactivo

Se desarrolló un dashboard en Tableau para explorar visualmente la eficiencia operativa:

👉 https://public.tableau.com/app/profile/oscar.aranda7717/viz/PF_Telecom/PFTelecom?publish=yes

---

## 📄 Presentación ejecutiva

Las conclusiones del análisis fueron sintetizadas en una presentación en PDF:

👉 https://docs.google.com/presentation/d/1vusGNCcoLnDp22063r5XBNHAoZ20WIoa/edit

---

## 📂 Archivos del proyecto

- 📓 `Proyecto_Final_CallMeMaybe.ipynb` – Análisis completo
- 📘 `README.md` – Documentación del proyecto

---

## ✅ Estado del proyecto

✔ Análisis exploratorio completado  
✔ Operadores ineficaces identificados  
✔ Hipótesis estadísticas validadas  
✔ Dashboard y presentación ejecutiva entregados  

---

## 🔗 Repositorio del proyecto

👉 *(https://github.com/utsa2004/proyectos-bootcamp-data-analyst-tripleten/tree/main/Proyecto%20FInal%20Sprint%2014/14.4%20Proyecto%20CallMeMaybe)*

---


## 🧠 Nota final

Este proyecto demuestra la capacidad de **integrar análisis exploratorio, estadística aplicada y visualización** para resolver un problema real de negocio. La metodología empleada permite no solo diagnosticar ineficiencias operativas, sino también **fundamentar decisiones estratégicas con evidencia cuantitativa**, un enfoque clave en proyectos de analítica profesional.

