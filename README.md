# 📞 Telco Customer Churn Prediction (Logistic Regression)

This project predicts customer churn using the Telco dataset. It includes data cleaning, feature engineering, logistic regression modeling, and performance visualization (confusion matrix and ROC curve).

---

## 📊 Dataset

- Source: IBM Telco Churn Dataset
- Size: ~7,000 customers
- Target: `Churn` (Yes/No → 1/0)
- Features: Customer demographics, account info, usage, service type

---

## 🔧 Pipeline Overview

### 1. Data Cleaning
- Converted `TotalCharges` to numeric
- Filled missing values
- One-hot encoded categorical variables
- Scaled numerical columns

### 2. Modeling
- Trained `LogisticRegression` on clean data
- Evaluated with:
  - Accuracy, Precision, Recall, F1
  - Confusion Matrix
  - ROC Curve / AUC

---

## ✅ Results

| Metric               | Value  |
|----------------------|--------|
| Accuracy             | 82.19% |
| Precision (Churn=1)  | 69%    |
| Recall (Churn=1)     | 60%    |
| F1-Score (Churn=1)   | 64%    |
| AUC (ROC)            | 0.86   |


---

## 📈 Visuals

### Confusion Matrix  
![image](https://github.com/user-attachments/assets/89326f43-dbaf-45b4-a306-2e6546bc9b00)


### ROC Curve  
![image](https://github.com/user-attachments/assets/48121615-00e6-4bb5-a361-48977f3eca16)


---

## 🧠 Key Learnings

- Logistic regression performs well on churn if data is cleaned properly
- `TotalCharges`, `tenure`, and `Contract` features have strong signal
- AUC of 0.86 shows real predictive power

---

## 💻 Requirements

```bash
pandas
numpy
matplotlib
seaborn
sc
