
# Churn Prediction ML Project

## 🚀 Project Overview

This project focuses on **predicting customer churn** for a telecom company using **machine learning models**. Customer churn prediction helps businesses **identify customers likely to leave** and take **proactive retention actions**.

We implemented and compared three models:

* **Random Forest** – Ensemble tree-based model, robust and interpretable.
* **Logistic Regression** – Linear model, interpretable, outputs probabilities.
* **XGBoost** – Gradient boosting model, highly accurate for tabular data.

The project also includes **visualizations and business-oriented simulations** to transform model predictions into actionable insights.

---

## 📂 Dataset

The dataset used is the **Telco Customer Churn dataset**, which contains:

* Customer demographics: gender, senior citizen status, partner, dependents.
* Service information: tenure, phone service, internet service, contract type, payment method.
* Billing information: MonthlyCharges, TotalCharges.
* Target variable: `Churn` (0 = retained, 1 = churned).

---

## 🛠️ Data Preparation

* **Missing values** handled (TotalCharges converted to numeric and NaNs filled with median).
* **Categorical features** encoded using one-hot encoding or 0/1 encoding.
* **Numeric features** standardized using `StandardScaler` (`tenure`, `MonthlyCharges`, `TotalCharges`) to have mean ~0 and std ~1.
* Dataset split into **train and test sets** to avoid data leakage.

---

## 📊 Models & Results

| Model               | Accuracy | Precision (Churn) | Recall (Churn) | F1-Score (Churn) |
| ------------------- | -------- | ----------------- | -------------- | ---------------- |
| Logistic Regression | 0.78     | 0.62              | 0.45           | 0.53             |
| Random Forest       | 0.78     | 0.63              | 0.46           | 0.54             |
| XGBoost             | 0.78     | 0.60              | 0.51           | 0.55             |

**Confusion Matrix Example (XGBoost)**:

```
[[911 124]
 [185 189]]
```

* **Interpretation:**

  * True Positives (189) → correctly predicted churned customers.
  * True Negatives (911) → correctly predicted retained customers.
  * False Positives / Negatives → errors to consider for business actions.

---

## 📈 Visualizations & Simulation

* **Prediction distribution:** GIF or images showing churn probability for customers.
* **Decision-making simulation:** Highlighted high-risk customers with suggested actions to reduce churn.
* Visualizations are designed to **communicate model results to business stakeholders**, not just data scientists.

---

## 💡 Business Insights / Decision Making

1. Customers with **high MonthlyCharges and short tenure** are most likely to churn → target them with retention offers.
2. Internet service type (Fiber optic) correlates with churn → improve service quality or bundle offers.
3. Probabilistic predictions allow the **marketing team to prioritize interventions** and **reduce churn cost-effectively**.
4. Simulations can be integrated into dashboards for **real-time retention strategy**.

---

## 🛠️ Technologies

* Python 3.x
* pandas, numpy, matplotlib, seaborn
* scikit-learn (Logistic Regression, Random Forest)
* xgboost
* Jupyter Notebook

---

## 📁 Repository Structure

```
Churn_Prediction_ML_Project/
│
├─ Machine_Learning_Predictive_Model.ipynb  # Notebook with code, preprocessing, modeling, visualizations
├─ WA_Fn-UseC_-Telco-Customer-Churn.csv    # Dataset
├─ churn_simulation.gif                     # Simulation GIF for LinkedIn/business presentation
├─ README.md                                # Project description and results
├─ .gitignore                               # Git ignore file
└─ LICENSE                                  # MIT license
```

---

## 📌 How to Run

1. Clone the repository:

```bash
git clone https://github.com/SalsabilRouahi/Churn_Prediction_ML_Project-.git
```

2. Open `Machine_Learning_Predictive_Model.ipynb` in Jupyter Notebook.
3. Run all cells to see preprocessing, modeling, results, and visualizations.

---

## 📌 Keywords for GitHub

`machine-learning`, `churn-prediction`, `python`, `xgboost`, `random-forest`, `logistic-regression`, `business-intelligence`, `decision-making`

---


