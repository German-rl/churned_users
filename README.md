# Waze User Churn Prediction 🚗📉

Predicting user churn in the Waze navigation app using machine learning models and class imbalance techniques.

## 📊 Project Overview

User retention is critical for navigation platforms like Waze.  
This project predicts which users are likely to churn based on behavioral and engagement data.

The analysis extends the Google Data Analytics Certificate case study by incorporating advanced modeling and class-imbalance handling techniques.

## 🎯 Business Objective

Identify users at risk of churn to enable:

- targeted retention campaigns  
- personalized engagement strategies  
- proactive product interventions  

Since missing churned users is costly, **recall and F1-score are prioritized over accuracy**.

---

## 🧠 Modeling Approach

Three models were trained and compared:

- XGBoost
- Random Forest
- Balanced Random Forest (class-imbalance optimized)

Evaluation metrics:

- Accuracy
- Recall
- F1-score
- ROC-AUC

---

## 📈 Model Performance

| Model | Accuracy | Recall | F1-score | ROC-AUC |
|------|---------|--------|---------|--------|
| XGBoost | 0.78 | 0.22 | 0.26 | 0.66 |
| Random Forest | 0.81 | 0.09 | 0.15 | 0.71 |
| **Balanced Random Forest** | 0.64 | **0.72** | **0.41** | **0.72** |

---

## ✅ Key Findings

- Standard models optimized for accuracy failed to detect churners.
- Balanced Random Forest dramatically improved churn detection.
- Recall increased from **0.09 → 0.72** vs Random Forest.
- F1-score nearly tripled vs XGBoost.

👉 For churn-risk identification, **Balanced Random Forest is the most effective model**.

---

## 🧾 Model Selection Guidance

- **Churn detection priority → Balanced Random Forest**
- **Balanced trade-off / false positives costly → XGBoost**

---

## 🛠️ Tech Stack

- Python
- pandas
- scikit-learn
- imbalanced-learn
- XGBoost
- matplotlib / seaborn

---
