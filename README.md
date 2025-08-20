# 📊 TelecomX – Predicción de Cancelación de Clientes (Churn)

## 🚀 Introducción
La cancelación de clientes (**Churn**) es uno de los mayores desafíos para empresas de telecomunicaciones.  
Este proyecto busca **predecir qué clientes están en riesgo de cancelar** su servicio, utilizando modelos de Machine Learning y analizando los factores que más influyen en la decisión de los usuarios.

---

## 📂 Dataset
- **Fuente:** Datos de clientes de una empresa de telecomunicaciones.  
- **Variable objetivo:** `Churn` (1 = Canceló, 0 = No canceló).  
- **Variables incluidas:**
  - Datos demográficos
  - Tipo de contrato
  - Consumo de servicios
  - Tiempo con la compañía
  - Gastos mensuales y totales

---

## ⚙️ Metodología
1. **Análisis exploratorio de datos (EDA)**
   - Matriz de correlación.
   - Relación de variables clave con la cancelación.
   - Visualizaciones con `boxplots`, `scatter plots` y `heatmaps`.

2. **Preprocesamiento**
   - Normalización de variables numéricas.
   - Codificación de variables categóricas.
   - División en **train (70%) y test (30%)**.

3. **Modelos Entrenados**
   - **Regresión Logística** (con normalización).
   - **Random Forest Classifier** (sin normalización).

4. **Evaluación**
   - Exactitud (Accuracy)
   - Precisión
   - Recall
   - F1-score
   - Matriz de confusión
   - ROC-AUC

---

## 📈 Resultados de Modelos

### 🔹 Regresión Logística
- Desempeño bueno pero menos robusto que Random Forest.
- Métricas balanceadas, con capacidad de explicar la relación de cada variable con el Churn.

### 🔹 Random Forest
- **Mejor desempeño global (100% en el set de prueba)**.
- Mayor capacidad de capturar interacciones no lineales.
- Posible **overfitting** debido al resultado perfecto (requiere validación cruzada).

---

## 🌟 Importancia de Variables
Según el modelo **Random Forest**, las variables más influyentes en la cancelación fueron:

1. **Tiempo de contrato** ⏳  
   Clientes con contratos cortos presentan mayor probabilidad de cancelar.

2. **Gasto total** 💰  
   Clientes con bajo gasto total suelen ser más propensos a irse.

3. **Gastos mensuales** 📉  
   Factores relacionados con la percepción de valor del servicio.

---

## 🧐 Conclusiones
- Los modelos muestran que **tipo de contrato, tiempo con la empresa y gasto total** son factores determinantes en la cancelación.
- El **Random Forest** presentó un desempeño excelente, pero el resultado perfecto sugiere validar con **nuevos datos** para confirmar la generalización.
- La **Regresión Logística** es útil para interpretar relaciones directas entre variables y la cancelación.

---

## 💡 Estrategias de Retención
1. **Contratos a largo plazo**  
   Incentivar contratos anuales o bianuales con beneficios adicionales.

2. **Programas de fidelización**  
   Descuentos progresivos para clientes con mayor tiempo de permanencia.

3. **Segmentación de clientes en riesgo**  
   Usar el modelo predictivo para identificar clientes con bajo gasto total y ofrecer paquetes personalizados.

4. **Optimización de precios y servicios**  
   Ajustar tarifas o agregar servicios de valor agregado para clientes con alta probabilidad de cancelación.

---

## 🛠️ Tecnologías Utilizadas
- **Python 3**
- **Pandas, Numpy**
- **Scikit-learn**
- **Matplotlib, Seaborn**

---
