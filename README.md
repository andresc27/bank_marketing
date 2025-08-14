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
- Entrenar y evaluar modelos de regresión logística y Neural Networks (NN).
- Comparar desempeño con y sin selección de variables.

**English:**
- Analyze and preprocess the data.
- Identify the most relevant features using correlation and mutual information.
- Train and evaluate logistic regression and Neural Networks (NN) models.
- Compare performance with and without feature selection.

---

## 🛠️ Tecnologías utilizadas / Technologies Used

- Python 3
- Pandas, NumPy
- Scikit-learn
- TensorFlow / Keras
- Matplotlib, Seaborn

---

## 🧪 Entrenamiento y Evaluación / Training and Evaluation

- División de datos en conjuntos de entrenamiento, validación y prueba.
- Escalado de características usando `StandardScaler`.
- Manejo de desbalance de clases con `class_weight`.
- Ajuste de umbral de decisión para priorizar la detección de clientes potenciales.
- Comparación de modelos:
  - **Logistic Regression** con selección de hiperparámetros (`C`) y balance de clases.
  - **Neural Network** con regularización, normalización por lotes y `Dropout`.

---

## 📊 Resultados / Results

**Logistic Regression:**

- Accuracy: 0.79
- Positive class (suscriptores):
  - Precision: 0.35
  - Recall: 0.95
  - F1-score: 0.51
- Negative class (no suscriptores):
  - Precision: 0.99
  - Recall: 0.77
- AUC ≈ 0.935

**Neural Network:**

- Accuracy: 0.84
- Positive class (suscriptores):
  - Precision: 0.41
  - Recall: 0.92
  - F1-score: 0.57
- Negative class (no suscriptores):
  - Precision: 0.99
  - Recall: 0.83
- AUC ≈ 0.901

**Observaciones:**

- La Neural Network mejora la **exactitud global**, la **precisión** y el **F1-score** de la clase positiva (clientes que se suscriben), mientras mantiene un **recall alto** para detectar clientes interesados.
- Logistic Regression mantiene ligeramente un AUC más alto, mostrando buena discriminación, pero con menor balance entre precisión y recall para detectar verdaderos suscriptores.
- Ajustar el umbral de decisión permite reducir falsos negativos, maximizando la captación de clientes potenciales.

---

## 📌 Conclusiones / Conclusions

**Español:**

- Es posible mejorar la detección de clientes potenciales usando Neural Networks, ajustando el umbral y manejando el desbalance de clases.
- La NN ofrece un mejor equilibrio entre precisión y recall para la clase positiva y mantiene alta exactitud para la clase negativa (reducimos falsos negativos y falsos positivos).
- Logistic Regression sigue siendo una opción interpretable y eficiente con desempeño sólido.

**English:**

- Potential customer detection can be improved using Neural Networks by adjusting the threshold and handling class imbalance.
- The NN provides a better balance between precision and recall for the positive class while maintaining high accuracy for the negative class.
- Logistic Regression remains an interpretable and efficient option with solid performance.

---

## ✍️ Autor / Author

- Nombre / Name: Andrés C

