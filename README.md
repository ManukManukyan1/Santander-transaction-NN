# Santander-transaction-NN

# 🧠 Tabular Binary Classification with Neural Networks

![Python](https://img.shields.io/badge/Python-3.9+-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-orange)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-MLP-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview
This project tackles a **binary classification problem on tabular data** using a **deep neural network (MLP)** built with **TensorFlow/Keras**.

The pipeline includes:
- Feature scaling
- Class imbalance handling
- Regularization techniques
- Learning rate scheduling
- AUC-based evaluation

This approach is suitable for datasets similar to the **Santander Customer Transaction Prediction** competition.

---

## 📊 Dataset
The dataset consists of:
- **200 numerical features**
- **Binary target variable (`target`)**
- An identifier column (`ID_code`) removed during preprocessing

---

## 🧠 Methodology
1. Remove identifier columns
2. Train / validation split
3. Feature scaling using **StandardScaler**
4. Build a **multi-layer perceptron**
5. Handle class imbalance using **class weights**
6. Train with:
   - Early stopping
   - Learning rate reduction
7. Generate probability predictions for submission

---

## 🏗 Model Architecture
- Dense (512) + BatchNorm + Dropout
- Dense (256) + BatchNorm + Dropout
- Dense (128) + BatchNorm + Dropout
- Output layer: **Sigmoid**

**Optimizer:** Adam  
**Loss:** Binary Crossentropy  
**Metric:** AUC  

---

## 🛠 Technologies Used
- Python
- Pandas & NumPy
- Scikit-learn
- TensorFlow / Keras
- Matplotlib & Seaborn
