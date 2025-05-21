# 🏠 Boston Housing Price Prediction Using Deep Learning

This project focuses on predicting housing prices in Boston using deep learning techniques. The model is built using TensorFlow/Keras and trained on the Boston Housing dataset. It leverages a neural network to estimate continuous values (house prices), making it a regression problem.

---

## 🎯 Project Objective

To develop and evaluate a neural network model that can predict the median value of owner-occupied homes in Boston suburbs based on various input features such as crime rate, number of rooms, and proximity to employment centers.

---

## 🧾 Dataset Description

- **Dataset:** Boston Housing dataset (`tensorflow.keras.datasets.boston_housing`)
- **Features:** 13 numerical attributes per data point, including:
  - CRIM: Per capita crime rate by town
  - RM: Average number of rooms per dwelling
  - LSTAT: % lower status of the population
  - ... (total 13 features)
- **Target:** Median value of owner-occupied homes (in $1000s)

---

## 🧱 Model Architecture

### Model 1
- `Dense(64, activation='relu')`
- `Dense(64, activation='relu')`
- `Dense(1)` – output layer for regression

### Model 2 (Deeper Architecture)
- `Dense(64, activation='relu')`
- `Dense(128, activation='relu')`
- `Dense(256, activation='relu')`
- `Dense(128, activation='relu')`
- `Dense(256, activation='relu')`
- `Dense(1)` – output layer

> Both models were evaluated using **Mean Absolute Error (MAE)** and **K-Fold Cross Validation**.

---

## ⚙️ Training Process

- **Loss Function:** Mean Squared Error (MSE)
- **Metric:** Mean Absolute Error (MAE)
- **Validation:** 4-fold cross-validation
- **Optimizer:** SGD (Stochastic Gradient Descent)
- **Epochs:** 130
- **Batch Size:** 16

---

## 📊 Visualizations

- **Model Summary Diagrams**  
  Architecture diagrams showing the number of layers and parameters used.

- **Training Curves**  
  MAE vs. Epochs plots show convergence trends.

- **Validation Results**  
  Per-fold MAE values plotted to compare model consistency across different validation sets.

  

---

## 🧪 Results

- Average MAE after 4-fold validation was satisfactory for both models.
- Deeper architecture improved generalization slightly, with reduced validation error.
- MAE decreased with additional layers, but overfitting was monitored using validation curves.

---


---

## 🧰 Tools Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Jupyter Notebook

---



