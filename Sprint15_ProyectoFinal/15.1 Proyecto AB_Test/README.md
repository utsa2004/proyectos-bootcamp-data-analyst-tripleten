# 🧪 A/B Testing – Evaluación de un Sistema de Recomendación  
**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción del proyecto
Una empresa internacional de comercio electrónico lanzó un experimento A/B para evaluar el impacto de un nuevo sistema de recomendaciones en la conversión del embudo de compras. El objetivo era determinar si el nuevo sistema mejoraba las tasas de conversión en al menos **10%**.

El experimento **`recommender_system_test`** comparó:

- **Grupo A (control):** sistema actual  
- **Grupo B (experimental):** sistema con recomendaciones mejoradas  

El análisis incluyó validación del experimento, exploración del embudo y pruebas estadísticas.

---

## 🎯 Objetivo principal
Determinar si el nuevo sistema de recomendaciones genera una mejora ≥10% en la conversión del embudo de compras.

---

## 🎯 Objetivos específicos
1. Analizar el impacto en las etapas del embudo:
   - `product_page`  
   - `product_cart`  
   - `purchase`
2. Validar consistencia del experimento (equilibrio A/B, ausencia de sesgos).  
3. Aplicar **pruebas Z de proporciones** para determinar significancia estadística.

---

## 🧠 Metodología

### **1. Validación del experimento**
- Revisión de coherencia interna  
- Balance entre grupos A/B  
- Ausencia de sesgos estructurales  

### **2. Análisis del embudo**
- Cálculo de tasas de conversión por etapa  
- Comparación completa entre grupos  
- Visualización del flujo del usuario  

### **3. Prueba estadística**
- Uso de `proportions_ztest`  
- Nivel de significancia: α = 0.05  
- Hipótesis:  
  - H₀: No hay diferencia entre A y B  
  - H₁: B mejora la conversión  

---

## 📊 Resultados
- El grupo B **no mostró mejoras significativas** en ninguna etapa del embudo.  
- Las diferencias no fueron estadísticamente significativas (**p > 0.05**).  
- El objetivo de mejora ≥10% **no se cumplió**.

---

## 💡 Conclusiones
- El nuevo sistema de recomendaciones **no aumenta la conversión** del embudo.  
- La prueba estuvo bien ejecutada y los datos fueron confiables.  
- Recomendaciones:  
  - No implementar el sistema actual  
  - Revisar el algoritmo de recomendación  
  - Analizar segmentos específicos de usuarios  
  - Ejecutar una nueva prueba A/B con ajustes  

---

## 🏆 Habilidades utilizadas
- Python (Pandas, NumPy, Seaborn, Plotly)  
- Estadística aplicada  
- A/B Testing (pruebas Z de proporciones)  
- Análisis de embudos  
- Limpieza y validación de datos  
- Visualización de datos  

---

## 📂 Archivos del proyecto
- `notebook_ab_test.ipynb` – Notebook con el análisis completo  
- `datasets/` – Datos utilizados  
- `plots/` – Visualizaciones generadas  
- `README.md` – Documentación del proyecto

---

## 🔗 Enlace al repositorio
*Agrega aquí la URL de GitHub una vez publicado.*

---
 
