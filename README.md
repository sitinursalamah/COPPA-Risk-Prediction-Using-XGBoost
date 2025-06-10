## 📱 COPPA Risk Prediction Using XGBoost

This repository contains my submission for the FINDIT 2025 competition.

### 🧠 Problem Overview

The task is a **binary classification** problem:
Predict whether a mobile app is **at risk of violating COPPA** (Children’s Online Privacy Protection Act) based on app metadata such as category, downloads, privacy policy, and developer information.

### 🎯 Target Variable

* `coppaRisk`

  * `True`: High risk of COPPA non-compliance
  * `False`: Low risk of COPPA non-compliance

### 🔍 Key Challenges

* Missing values (e.g., "ADDRESS NOT LISTED IN PLAYSTORE")
* Categorical feature encoding
* Imbalanced dataset
* Need for interpretability

### ⚙️ Model Used

* **XGBoost**
  Chosen for its high performance on structured data, ability to handle missing values, and feature importance interpretation.

#### 📊 Model Performance (AUC Score)

| Iteration | Validation AUC |
| --------- | -------------- |
| \[0]      | 0.86243        |
| \[50]     | 0.89328        |
| \[100]    | 0.89625        |
| \[113]    | 0.89668        |

**Final XGBoost AUC Score: 0.89685**


### 📈 Evaluation Metric

* **AUC (Area Under the ROC Curve)**
