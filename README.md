# 🚴 REGRESIÓN: IMPLEMENTA UNA RED NEURONAL CON NUMPY

[![Python](https://img.shields.io/badge/Python-3670A0?style=flat&logo=python&logoColor=ffdd54)](https://www.python.org/)  
[![Numpy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)](https://numpy.org/)  
[![Regresión](https://img.shields.io/badge/Regresi%C3%B3n-00BCD4?style=flat&logo=scikit-learn&logoColor=white)](https://es.wikipedia.org/wiki/An%C3%A1lisis_de_la_regresi%C3%B3n)  
[![Red Neuronal](https://img.shields.io/badge/Red%20Neuronal-5D3FD3?style=flat&logo=tensorflow&logoColor=white)](https://es.wikipedia.org/wiki/Red_neuronal_artificial)

Este proyecto es un ejercicio fundamental en **Deep Learning** que consiste en la **implementación de una Red Neuronal (NN) desde cero** utilizando exclusivamente la librería **NumPy**. El objetivo es resolver un problema de **Regresión**, prediciendo la cantidad de **bicicletas alquiladas** basándose en factores climáticos como la temperatura y el clima. Al no depender de *frameworks* de alto nivel como Keras o TensorFlow, se logra una comprensión profunda de la **lógica matemática interna** de cómo aprenden las redes.

---

## 🧠 Contenido del Proyecto

### 1️⃣ El Problema de Regresión
- **Objetivo:** Determinar el **número de bicicletas alquiladas** en un momento dado.
- **Variables de Entrada:** La predicción se basa en variables como el **clima** y la **temperatura**.
- **Regresión:** A diferencia de la clasificación (que predice categorías), la regresión predice un **valor continuo** (en este caso, un número de bicicletas).

### 2️⃣ Implementación "Desde Cero" con NumPy
El corazón del proyecto es construir manualmente todos los elementos de la Red Neuronal, sin abstracciones:

- **Estructura de la Red:** Se define la arquitectura con capas y el flujo de datos.
- **Función de Activación (Sigmoid):** Se implementa manualmente la función Sigmoid, crucial para introducir no linealidad en las capas.
- **Función de Pérdida (MSE):** Se calcula el Error Cuadrático Medio (MSE) para cuantificar la diferencia entre las predicciones y los valores reales.
- **Backpropagation:** El proceso de **propagación hacia atrás**, donde se ajustan los pesos de la red para minimizar el error, se implementa completamente con operaciones de NumPy.

### 3️⃣ Fases del Aprendizaje
El proyecto ilustra y ejecuta las dos fases esenciales del Deep Learning:

1.  **Forward Pass (Propagación Hacia Adelante):** Cálculo de la salida de la red.
2.  **Backward Pass (Propagación Hacia Atrás):** Cálculo de los gradientes y ajuste de **Pesos (Weights)** y **Bias (Sesgo)**.

---

## 🛠️ Librerías Utilizadas

| Librería | Uso principal |
|:---:|:---:|
| **NumPy** | **Implementación completa de la Red Neuronal**, cálculo de matrices, pesos y gradientes. |
| **Pandas** | Carga y preprocesamiento inicial de los datos de bicicletas. |
| **Matplotlib** | Visualización de los resultados y el proceso de entrenamiento. |
| **Scikit-learn** | División del dataset en conjuntos de entrenamiento y prueba (`train_test_split`). |

---

## 🎯 Objetivo del Proyecto
El objetivo principal es lograr una **comprensión fundamental y práctica** de los mecanismos de las Redes Neuronales. Al forzar la construcción manual de la red con NumPy, el proyecto asegura que el usuario entienda cómo se ejecutan internamente las matemáticas del **Deep Learning**, incluyendo la **función de pérdida**, la **propagación hacia adelante** y, lo más importante, el complejo proceso de **ajuste de pesos** mediante *Backpropagation*.

---

## 📈 Resultados Clave
- **Implementación Pura:** Se logra construir una Red Neuronal funcional (para un problema de regresión) utilizando **solo NumPy**, verificando la lógica matemática interna sin el uso de frameworks de alto nivel.
- **Visualización del Error:** Mediante el uso de Matplotlib, se **grafica la función de pérdida (MSE)** a través de las iteraciones (*epochs*), lo que demuestra cómo la red **aprende gradualmente** y el error se reduce con cada ajuste de pesos realizado por el *Backpropagation*.
- **Predicción de Valores Continuos:** El modelo demuestra la capacidad de **predecir un valor numérico continuo** (número de bicicletas), validando su aplicación en problemas de Regresión.
