# SUPER-STACK-Ensemble-for-Multiclass-Rheumatic-Disease-Diagnosis Using Clinical Data

## 🔍 Project Overview
Rheumatic diseases are a group of autoimmune and inflammatory disorders that present significant diagnostic challenges due to overlapping symptoms, heterogeneous clinical features, and complex laboratory markers. Early and accurate diagnosis is crucial for effective disease management and improved patient outcomes.

This project presents an end-to-end machine learning system for rheumatic disease prediction, combining ensemble learning, stacking models, and Explainable AI (SHAP) with an interactive Gradio web application to provide transparent, interpretable, and accurate predictions.

---

## 🎯 Problem Statement
Traditional diagnostic approaches rely heavily on expert interpretation of clinical and laboratory data, which can be time-consuming and subjective. The goal of this project is to automate early disease prediction while maintaining model interpretability to support clinical decision-making.

---

## 🚀 Solution Approach
The system follows a complete machine learning pipeline:
- Data cleaning and preprocessing
- Feature engineering based on clinical knowledge
- Handling class imbalance using SMOTEENN
- Training multiple machine learning models
- Ensemble and stacking-based model selection
- Explainable AI using SHAP
- Deployment through a Gradio-based web interface

---
## DATASET
The dataset used in this study is: “Diagnosis of Rheumatic and Autoimmune Diseases” Published in Data in Brief, 2025.

Mohammed Fadhil Mahdi et al. Diagnosis of rheumatic and autoimmune diseases dataset, Data in Brief, Volume 60, 2025, Article 111623 DOI: https://doi.org/10.1016/j.dib.2025.111623


## 🧠 Machine Learning Models Used
- Random Forest
- XGBoost
- LightGBM
- CatBoost
- Stacking Ensemble
- Super Stack (CatBoost + XGBoost + LightGBM)
- Stack (RF+ XGBoost)


The best-performing model is automatically selected and saved for deployment.

---

## 🛠️ Technology Stack

**Language**
- Python

**Libraries**
- Pandas, NumPy
- Scikit-learn
- XGBoost, LightGBM, CatBoost
- Imbalanced-learn
- SHAP (Explainable AI)
- Matplotlib
- Gradio

---

## 🧪 Feature Engineering
Key engineered features include:
- Inflammation Score (ESR + CRP)
- ESR to CRP Ratio
- Autoantibody Count
- Age Group Classification

These features enhance the model’s ability to capture clinically relevant patterns.

---

## ⚖️ Class Imbalance Handling
Medical datasets are often imbalanced. This project uses SMOTEENN, a hybrid over-sampling and under-sampling technique, to improve generalization across disease classes.

---

## 🔎 Explainable AI (SHAP)
- Global SHAP explanations identify important clinical features
- Local SHAP explanations explain individual predictions
- Improves interpretability for healthcare-related decision support

---

## 🌐 Web Application
The Gradio web interface allows users to:
- Input patient clinical details
- Receive predicted Autoimmunr disease
- View interpretable model behavior
- Support real-time inference

---

## 📁 Project Structure
```
Rheumatic-Disease-Prediction/
│
├── data/
│ └── Rheumatic-and-Autoimmune-Disease-Dataset.xlsx
│
├── artifacts/
│ ├── best_model.pkl
│ ├── scaler.pkl
│ ├── label_encoders.pkl
│ └── label_y.pkl
│
├── config.py
├── train.py
├── app.py
├── requirements.txt
├── README.md
└── .gitignore
```

## 📊 Output
## Model Performance Comparison

The following table compares the performance of all baseline models and the proposed SUPER STACK (CatBoost + XGBoost + LightGBM) in terms of Accuracy, Precision, Recall, and F1‑Score.
## ![OUTPUT](assests/image.png)

## Confusion Matrix
![OUTPUT](assests/confusion_matrix.png)

## Explainable predictions using SHAP

![OUPUT](assests/SHAP.jpg)

## Interactive Gradio-based user interface

![OUTPUT](assests/gradio_app.png)

## 🔮 Future Enhancements

- Multi-center and longitudinal clinical datasets

- Integration of imaging and genetic data

- Cloud deployment (AWS / Azure / GCP)

- Integration with Electronic Health Records (EHR)

- Model uncertainty estimatio

## 🧩 Conclusion

This project successfully demonstrates an automated and interpretable approach for the early diagnosis of autoimmune and rheumatic disorders using clinical data. By integrating robust data preprocessing, clinically informed feature engineering, and advanced ensemble learning techniques, the system achieves reliable and accurate disease classification. The use of stacking and super-stack models enhances predictive performance, while Explainable AI techniques (SHAP) ensure transparency by providing both global and local insights into model decisions. The deployment of the solution through a Gradio-based web interface enables real-time predictions and improves usability for non-technical users. Overall, this project highlights the potential of machine learning–driven decision support systems in healthcare and lays a strong foundation for future clinical applications.

bd6022e002b47fd9861bcb832685c7c7c2f5c1fe

