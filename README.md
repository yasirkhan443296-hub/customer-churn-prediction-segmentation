# customer-churn-prediction-segmentation
End-to-end ML project: Churn Prediction (XGBoost/RF), Customer Segmentation (KMeans), and Retention Recommendations | Python, Scikit-learn, SMOTE, PCA
# 🔄 Customer Churn Prediction + Segmentation + Retention Recommendation System



![Python](https://img.shields.io/badge/Python-3.10-blue)




![ML](https://img.shields.io/badge/Machine%20Learning-Scikit--learn-orange)




![Status](https://img.shields.io/badge/Status-Completed-green)



## 📌 Project Overview
A complete end-to-end Machine Learning project built on the **Telco Customer Churn Dataset**.
This project goes beyond simple churn prediction — it segments churned customers into meaningful 
groups and provides actionable retention strategies for each segment.

---

## 🎯 Business Problem
A telecom company is losing customers every month.
- **Who** is going to churn?
- **Why** are they leaving?
- **What** can we do to retain them?

This project answers all three questions.

---

## 🏗️ Project Architecture
---

## 📊 Dataset
- **Source:** Telco Customer Churn (Kaggle)
- **Size:** 7,043 rows × 21 columns
- **Target:** Churn (Yes/No)
- **Class Imbalance:** 73% No Churn, 27% Churn → Fixed with SMOTE

---

## 🔬 Project Components

### 1️⃣ Exploratory Data Analysis
- Churn distribution analysis
- Contract vs Churn
- Tenure vs Churn
- MonthlyCharges vs Churn
- PaymentMethod vs Churn
- Numerical feature distributions

### 2️⃣ Feature Engineering
- Created `tenure_group` feature (New / Mid / Loyal)
- Handled missing values in TotalCharges
- Label Encoding for categorical columns
- StandardScaler for numerical features
- SMOTE to fix class imbalance

### 3️⃣ Churn Prediction Models
| Model | Accuracy | ROC-AUC |
|---|---|---|
| Logistic Regression | ~78% | ~0.78 |
| Random Forest | ~92% | ~0.92 |
| XGBoost | ~93% | ~0.93 |

✅ Best Model: **XGBoost**

### 4️⃣ Customer Segmentation (KMeans)
Churned customers segmented into **5 clusters** using KMeans:

| Segment | Profile |
|---|---|
| New Low-Value Customers | Short tenure, low charges |
| Loyal Premium Customers | Long tenure, high charges |
| Mid-Tenure High Spenders | Mid tenure, high charges |
| New Price-Shocked Customers | Short tenure, very high charges |
| Mid-Tenure Low Spenders | Mid tenure, low charges |

### 5️⃣ Retention Recommendations
Rule-based retention strategy for each segment:

| Segment | Risk | Strategy |
|---|---|---|
| New Low-Value Customers | Medium | Onboarding Support + 10% discount |
| Loyal Premium Customers | Very High | VIP Loyalty Program + 20% discount |
| Mid-Tenure High Spenders | High | Annual contract upgrade + 15% off |
| New Price-Shocked Customers | Very High | 25% price reduction immediately |
| Mid-Tenure Low Spenders | Medium | Bundled services upsell |

---

## 🛠️ Tech Stack
| Category | Tools |
|---|---|
| Language | Python 3.10 |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn, XGBoost |
| Imbalance Handling | SMOTE (imbalanced-learn) |
| Clustering | KMeans, PCA |
| Model Saving | Joblib |

---

## 📁 Project Structure
