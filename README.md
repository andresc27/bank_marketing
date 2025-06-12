# Bank Term Deposit Prediction / Predicción de Depósitos a Plazo

Este proyecto utiliza técnicas de aprendizaje automático para predecir si un cliente aceptará un depósito a plazo, utilizando el dataset de marketing bancario disponible en el repositorio de UCI Machine Learning.

This project applies machine learning techniques to predict whether a customer will subscribe to a term deposit, using the Bank Marketing dataset from the UCI Machine Learning Repository.

---

## 📁 Dataset

- Fuente / Source: [UCI Machine Learning Repository - Bank Marketing Dataset](https://archive.ics.uci.edu/dataset/222/bank+marketing)
- Número de instancias / Number of instances: 45,211
- Características / Features: 16 atributos + 1 variable objetivo (`y`)
- Tarea / Task: Clasificación binaria (sí/no)

---

## 🎯 Objetivos / Objectives

**Español:**
- Analizar y preparar los datos.
- Identificar las variables más relevantes usando correlación e información mutua.
- Entrenar y evaluar modelos de regresión logística.
- Comparar desempeño con y sin selección de variables.

**English:**
- Analyze and preprocess the data.
- Identify the most relevant features using correlation and mutual information.
- Train and evaluate logistic regression models.
- Compare performance with and without feature selection.

---

## 🛠️ Tecnologías utilizadas / Technologies Used

- Python 3
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

---

## 🧪 Entrenamiento y Evaluación / Training and Evaluation

- División de datos en conjuntos de entrenamiento, validación y prueba.
- Escalado de características usando `StandardScaler`.
- Métrica principal: Accuracy
- Evaluación comparativa de dos modelos:
  - Modelo con todas las variables.
  - Modelo con variables seleccionadas por información mutua.

---

## 📊 Resultados / Results

- Ambos modelos lograron una precisión cercana al 91%.
- La selección de características permitió reducir la complejidad sin pérdida significativa de desempeño.
- El segundo modelo ofrece mayor interpretabilidad y puede ser útil en entornos donde la simplicidad del modelo es clave.

---

## 📌 Conclusiones / Conclusions

**Español:**
- Es posible construir modelos precisos con un subconjunto reducido de variables.
- La información mutua es útil para la selección de características en problemas de clasificación binaria.

**English:**
- Accurate models can be built using a reduced subset of features.
- Mutual information is useful for feature selection in binary classification tasks.

---

## 🚀 Cómo ejecutar / How to Run

1. Clona este repositorio:  
   `git clone https://github.com/tu_usuario/bank-term-deposit-prediction.git`
2. Instala los requerimientos:  
   `pip install -r requirements.txt`
3. Ejecuta el notebook en Jupyter:  
   `jupyter notebook bank_term_prediction.ipynb`

---

## ✍️ Autor / Author

- Nombre / Name: [Tu Nombre]
- Contacto / Contact: [Tu email o GitHub]

