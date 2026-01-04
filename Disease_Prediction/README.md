# 🩺 Heart Disease Prediction Model

This project predicts the likelihood of heart disease based on medical attributes using
Machine Learning classification techniques. The goal of this project is to assist
healthcare systems in early disease detection and risk assessment.

---

## Project Overview

Heart disease is one of the leading causes of death worldwide.  
Early detection can significantly improve treatment outcomes.

In this project, a machine learning pipeline is developed that:

 Handles missing values  
 Performs outlier capping using IQR  
 Scales numeric features  
 Encodes categorical features  
 Applies feature selection  
 Trains a Random Forest Classifier  

The model achieves strong performance with high Recall, making it suitable for
medical-risk prediction use cases.

---

## Dataset

The dataset contains patient health attributes such as:

- Age
- Sex
- Chest Pain Type
- Resting Blood Pressure
- Cholesterol Level
- Fasting Blood Sugar
- Resting ECG Results
- Maximum Heart Rate
- Exercise-Induced Angina
- ST Depression
- Slope of ST Segment
- Number of Major Vessels
- Thalassemia
- **Target (0 = No Disease, 1 = Disease)**

Target variable is binary (classification problem).

---

## Tech Stack

- Python
- Pandas, NumPy
- Scikit-Learn
- Random Forest Classifier
- Pipeline & ColumnTransformer

---

##  Model Pipeline

The preprocessing pipeline includes:

###  Numeric Features

- Median Imputation  
- IQR Outlier Capping  
- Standard Scaling  

###  Categorical Features

- Most Frequent Imputation  
- One-Hot Encoding  

###  Model

- RandomForestClassifier (`class_weight = balanced`)
- SelectFromModel Feature Selection

---

## Model Performance

| Metric | Score |
|------|------|
| Accuracy | 0.97 |
| Precision | 1.00 |
| Recall | 0.93 |
| F1-Score | 0.96 |
| ROC-AUC | 1.00 |

  High Recall ensures disease cases are rarely missed  
  Balanced performance across both classes

---

## Confusion Matrix

- True Negatives: 58  
- False Positives: 0  
- False Negatives: 3  
- True Positives: 42  

The model correctly identifies most heart disease patients.

---

## Future Improvements

- Hyperparameter tuning
- Cross-validation
- Precision-Recall curve analysis
- SHAP explainability
- Deploy as a web API / Streamlit app

---

## Project Structure

- Disease_prediction_model.ipynb
- heart.csv
- README.md