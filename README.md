# 📊 Telecom X – Predicción de Cancelación (Churn)

## 📖 Descripción
Este proyecto aborda el problema de la **predicción de cancelación de clientes (Churn)** en la empresa ficticia **Telecom X**.  

Se desarrolla un pipeline completo de **Machine Learning**, desde la preparación de datos hasta la evaluación de modelos, con el objetivo de anticipar qué clientes tienen mayor probabilidad de dejar el servicio.  

---

## ⚙️ Flujo del Proyecto
1. **Preprocesamiento de datos**  
   - Limpieza de valores nulos  
   - Codificación de variables categóricas  
   - Normalización de variables numéricas  

2. **Análisis exploratorio (EDA)**  
   - Distribución de variables  
   - Correlaciones  
   - Identificación de patrones de cancelación  

3. **Modelado predictivo**  
   - Modelos entrenados:  
     - Dummy Regressor (baseline)  
     - Regresión logística  
     - Árboles de decisión / Random Forest  
   - Comparación de métricas  

4. **Evaluación**  
   - Accuracy, Precision, Recall, F1-Score  
   - ROC-AUC y curva ROC  
   - Importancia de variables  

5. **Conclusión estratégica**  
   - Identificación de factores clave que influyen en la cancelación  
   - Recomendaciones de negocio  

---

## 📈 Resultados principales
- Se estableció un **modelo baseline** con `DummyRegressor`.  
- Los modelos entrenados superaron significativamente al baseline en métricas de clasificación.  
- Las variables más influyentes en la cancelación fueron:  
  - **Tenure (antigüedad del cliente)**  
  - **MonthlyCharges (cargo mensual)**  
  - **Contract (tipo de contrato)**  
- Se concluyó que clientes con **contratos cortos y altos costos mensuales** presentan mayor riesgo de cancelar.  

