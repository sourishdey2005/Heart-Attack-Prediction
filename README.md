# Heart-Attack-Prediction
Heart Attack Prediction



[![Python](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/)  
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.8+-orange.svg)](https://www.tensorflow.org/)  
[![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red.svg)](https://keras.io/)  
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)  





# 🫀 Heart Attack Prediction System  

A **lightweight deep learning model** for predicting **heart attack risk** using standard clinical diagnostic data. Built with **TensorFlow/Keras**, the model is designed for **high accuracy**, **real-world deployment**, and **edge/mobile environments**.  

---

## 📊 Model Performance & Specifications  

| Metric        | Performance | Description |
|---------------|-------------|-------------|
| **Accuracy**  | ≥90%        | Correct predictions on test dataset |
| **AUC-ROC**   | ≥0.90       | Excellent discrimination ability |
| **Model Size**| <100 KB     | Extremely lightweight for fast deployment |
| **Inference** | <1 ms       | Near real-time prediction capability |
| **Format**    | `.h5`       | Compatible with all TensorFlow platforms |

---

## ✅ Evaluation Metrics  

| Evaluation Metric | Target Value | Interpretation |
|-------------------|--------------|----------------|
| **Accuracy**      | ≥0.90        | 90%+ correct predictions |
| **Precision**     | ≥0.85        | Low false positive rate |
| **Recall**        | ≥0.85        | Low false negative rate |
| **F1-Score**      | ≥0.85        | Balanced precision/recall |
| **AUC-ROC**       | ≥0.90        | Excellent classification ability |

**Confusion Matrix Interpretation**:  
- **True Positives (TP):** Correctly identified heart disease cases  
- **True Negatives (TN):** Correctly identified healthy cases  
- **False Positives (FP):** Healthy patients flagged as at-risk  
- **False Negatives (FN):** Heart disease cases missed  

---

## 🚀 Features  

- ✅ **End-to-end ML pipeline** (preprocessing + prediction)  
- ✅ **Handles missing values** (saved imputer)  
- ✅ **Feature scaling & encoding** included  
- ✅ **Lightweight model (<100 KB)** for mobile/edge deployment  
- ✅ **Ready-to-use prediction interface** (`HeartAttackKerasPredictor`)  
- ✅ **Batch & single predictions supported**  
- ✅ **Visualization & metrics provided**  

---

## 🏗️ Model Architecture  

A **lightweight Multi-Layer Perceptron (MLP)**:  

| Layer            | Parameters             | Activation |
|------------------|------------------------|------------|
| **Input Layer**  | 16+ features (after encoding) | N/A |
| **Hidden Layer 1** | 16 neurons           | ReLU |
| **Hidden Layer 2** | 8 neurons            | ReLU |
| **Output Layer** | 1 neuron (binary)     | Sigmoid |

- **Total Parameters:** ≈ 500  
- **Optimizer:** Adam (lr=0.005)  
- **Loss Function:** Binary Cross-Entropy  
- **Training:** 50 epochs  

---

## 📁 Project Structure  
heart_model_keras_h5/
├── heart_model.h5 # Trained Keras model
├── imputer.pkl # Missing value imputer
├── scaler.pkl # Feature scaler
├── feature_columns.pkl # Expected features
├── model_type.txt # Model type info
├── model_performance_keras_h5.png # Performance visualization
└── usage_example.py # Usage example



---

## 🛠️ Requirements  

- Python 3.7+  
- TensorFlow 2.8+  
- scikit-learn 1.0+  
- pandas 1.3+  
- numpy 1.21+  
- matplotlib 3.5+  
- seaborn 0.11+  
- joblib 1.1+


📋 Input Features
Feature	Description	Range/Values
age	Age in years	29–77
sex	Gender	1 = Male, 0 = Female
cp	Chest pain type	1–4
trestbps	Resting blood pressure (mm Hg)	94–200
chol	Serum cholesterol (mg/dL)	126–564
fbs	Fasting blood sugar	1 = >120, 0 = ≤120
restecg	Resting ECG results	0–2
thalach	Max heart rate	71–202
exang	Exercise-induced angina	1 = Yes, 0 = No
oldpeak	ST depression	0.0–6.2
slope	ST segment slope	1–3
ca	Major vessels colored	0–3

Categorical Feature Details:

cp: 1 = Typical angina, 2 = Atypical, 3 = Non-anginal, 4 = Asymptomatic

restecg: 0 = Normal, 1 = ST-T abnormality, 2 = LV hypertrophy

slope: 1 = Upsloping, 2 = Flat, 3 = Downsloping




**Install dependencies:**  

```bash
pip install tensorflow scikit-learn pandas numpy matplotlib seaborn joblib
```



MIT License
Copyright (c) 2024
Permission is hereby granted, free of charge, to any person obtaining a copy of this software...
