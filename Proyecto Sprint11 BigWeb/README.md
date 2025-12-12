# 🛒 Proyecto Sprint 11 – Análisis de Negocio para Tienda Online BigWeb  
**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción general

Este proyecto consiste en un análisis integral de un **experimento A/B** realizado por **BigWeb**, una tienda online ficticia interesada en mejorar sus ingresos mediante cambios en su plataforma.  
El objetivo central es evaluar si las modificaciones aplicadas al grupo experimental generan mejoras significativas en métricas clave del negocio.

El análisis combina **priorización de hipótesis**, **preparación de datos**, **evaluación estadística** y **recomendaciones accionables**, integrando metodologías utilizadas por equipos reales de marketing, producto y data science.

---

## 🎯 Objetivo del Proyecto

El propósito principal es **evaluar, con evidencia estadística**, si los cambios del experimento A/B conducen a:

- Aumentar la tasa de conversión.  
- Incrementar el ingreso promedio por pedido.  
- Mejorar los ingresos totales de BigWeb.  

Adicionalmente, se busca:

- Priorizar hipótesis de alto impacto mediante ICE y RICE.  
- Identificar oportunidades para optimizar el desempeño comercial de la plataforma.  
- Promover decisiones estratégicas basadas en datos dentro del negocio.

---

## 🔍 Estructura del Proyecto

El proyecto se desarrolló en **cuatro etapas principales**:

---

### 📌 **1. Priorización de hipótesis**

Antes del análisis, se revisó una lista de hipótesis generadas por marketing y se priorizaron usando:

- **ICE (Impact – Confidence – Ease)**  
- **RICE (Reach – Impact – Confidence – Effort)**  

Esto permitió seleccionar aquellas ideas con mayor potencial de generar valor comercial.  
La **Hipótesis 7 ("Agregar un formulario de suscripción en todas las páginas principales")** resultó la mejor posicionada.

---

### 📁 **2. Preparación y validación de datos**

Se trabajó con múltiples fuentes de datos relacionadas con usuarios, pedidos y sesiones.  
Las tareas clave incluyeron:

- Eliminación de duplicados y valores nulos.  
- Ajustes de tipos de datos y formatos.  
- Integración de tablas a nivel usuario y pedido.  
- Validación de consistencia y calidad para asegurar un análisis confiable.

Para el análisis se emplearon las siguientes librerías:

```python
import pandas as pd
import numpy as np
from matplotlib import pyplot as plt
import seaborn as sns
from scipy import stats as st
