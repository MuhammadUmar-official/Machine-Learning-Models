# Credit Scoring Model (Machine Learning)

This project predicts whether a customer is likely to default on a credit loan
based on financial and demographic attributes. The goal of this project is to
help financial institutions assess credit risk more effectively.

---

## Project Overview

Credit scoring plays a critical role in banking and lending systems.  
An accurate risk prediction model helps:

Reduce financial losses  
Prevent high-risk lending  
Improve loan approval decisions  

In this project, a full machine learning pipeline is built that:

 Handles missing values  ss
 Performs outlier capping  
 Scales numeric features  
 Encodes categorical features  
 Applies feature selection  
 Trains a classification model for credit risk prediction

---

## Dataset Description

The dataset contains customer attributes such as:

- Age  
- Gender  
- Employment Status  
- Credit Amount  
- Duration of Credit  
- Housing Status  
- Account Balance  
- Payment History  
- Number of Existing Credits  
- Purpose of Loan  

🎯 **Target Variable**

- 0 = Good Credit (Low Risk)
- 1 = Bad Credit (High Risk / Default Risk)

This is a **binary classification problem**.

---

## Tech Stack

- Python
- Pandas, NumPy
- Scikit-Learn
- Random Forest Classifier
- ColumnTransformer + Pipeline
- SelectFromModel Feature Selection

---

## Model Pipeline

### Numeric Features Processing

- Median Imputation  
- IQR Outlier Capping  
- Standard Scaling  

### Categorical Features Processing

- Most Frequent Imputation  
- One-Hot Encoding  

### Model Used

- RandomForestClassifier  
- Class Weight = balanced (to handle imbalanced data)
- Feature Selection using SelectFromModel

---

## Model Evaluation

Performance metrics calculated:

- Accuracy  
- Precision  
- Recall  
- F1-Score  
- ROC-AUC Score  
- Confusion Matrix

The model shows good balance between:

 Risk detection  
 False positive control  
 Credit approval fairness

(This section can be updated with your actual metric values.)

---

## Business Relevance

This model can be used for:

✔ Loan approval decision support  
✔ Customer risk profiling  
✔ Default probability estimation  
✔ Financial risk analytics  

It helps organizations:

- Reduce non-performing loans  
- Improve lending policies  
- Automate credit scoring systems  

---

## folder structure

- credit_scoring_model.ipynb
- german_credit_cleaned.csv
- README.md
