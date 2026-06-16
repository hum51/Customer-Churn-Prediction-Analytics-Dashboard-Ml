# Customer-Churn-Prediction-Analytics-Dashboard-Ml
ML system for customer churn prediction using Logistic Regression &amp; Random Forest. Includes EDA, feature engineering, customer segmentation, risk categorization &amp; business insights dashboard.

📋 Table of Contents
- [🎯 Objective](#-objective)
- [📊 Dataset](#-dataset)
- [🔧 Tech Stack](#-tech-stack)
- [⚙️ Project Pipeline](#️-project-pipeline)
- [📈 Visualizations](#-visualizations)
- [🤖 ML Models & Results](#-ml-models--results)
- [🎲 Prediction System](#-prediction-system)
- [💡 Business Insights](#-business-insights)
- [📁 File Structure](#-file-structure)
- [🚀 How to Run](#-how-to-run)
- [👤 Author](#-author)

---

## 🎯 Objective

Build an **end-to-end ML system** that analyzes customer behavior data, generates actionable business insights, and predicts churn probability using machine learning models.

> *"Transform raw customer data into actionable insights and predictions."*

---

## 📊 Dataset

| Property | Details |
|----------|---------|
| **Source** | Telco Customer Churn Dataset |
| **Records** | 7,043 customers |
| **Features** | 21 attributes |
| **Target** | Churn (Yes/No) |
| **Churn Rate** | 26.5% |

**Key Features:**
- 👤 Demographics: Gender, SeniorCitizen, Partner, Dependents
- 📅 Account Info: Tenure, Contract, PaymentMethod
- 📞 Services: Phone, Internet, Streaming, TechSupport
- 💰 Financial: MonthlyCharges, TotalCharges

---

## 🔧 Tech Stack

| Category | Tools |
|----------|-------|
| **Languages** | Python 3.8+ |
| **Data Processing** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Machine Learning** | Scikit-Learn |
| **Environment** | Jupyter Notebook |

---

## ⚙️ Project Pipeline
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│  📥 Data Load   │ →  │  🧹 Cleaning    │ →  │  📊 EDA         │
│  & Inspection   │    │  & Preprocessing│    │  & Statistics   │
└─────────────────┘    └─────────────────┘    └─────────────────┘
↓
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│  🛠️ Feature     │ →  │  📈 Data        │ →  │  🎲 Customer    │
│  Engineering    │    │  Visualization  │    │  Segmentation   │
└─────────────────┘    └─────────────────┘    └─────────────────┘
↓
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│  🤖 Model       │ →  │  🎯 Prediction  │ →  │  💡 Business    │
│  Training &     │    │  & Risk Scoring │    │  Insights Report│
│  Evaluation     │    │                 │    │                 │


## 📈 Visualizations

### 📊 Dashboard 1: Business Analytics (12 Charts)
- 🥧 Churn Distribution
- 📉 Revenue Trends by Tenure
- 🏷️ Customer Segmentation
- 📋 Churn by Contract Type
- 💳 Churn by Payment Method
- 🌐 Churn by Internet Service
- 🔥 Feature Correlation Heatmap
- 💵 Monthly Charges Distribution
- 📅 Tenure Distribution
- 🛡️ Service Subscription Comparison
- 🎯 Segment-wise Churn Rate
- 💎 Spending Category Analysis

### 📊 Dashboard 2: Model Evaluation (6 Charts)
- 🔵 Confusion Matrix — Logistic Regression
- 🟢 Confusion Matrix — Random Forest
- 📈 ROC Curve Comparison
- 📊 Model Performance Bar Chart
- 🔑 Top 15 Feature Importances
- 🎲 Churn Probability Distribution

---

## 🤖 ML Models & Results

### Model 1: Logistic Regression
| Metric | Score |
|--------|-------|
| Accuracy | 0.7557 |
| Precision | 0.5224 |
| Recall | 0.7659 |
| F1 Score | 0.6213 |
| ROC-AUC | 0.8351 |

### Model 2: Random Forest ⭐ (Best Model)
| Metric | Score |
|--------|-------|
| Accuracy | 0.7994 |
| Precision | 0.6502 |
| Recall | 0.7092 |
| F1 Score | 0.6785 |
| ROC-AUC | 0.8362 |

> ✅ **Random Forest selected as final model** for prediction system

---

## 🎲 Prediction System

### Risk Categories

| Risk Level | Probability Range | Count | Actual Churn Rate |
|------------|-------------------|-------|-------------------|
| 🟢 **Low Risk** | < 40% | 4,265 | 7.8% |
| 🟡 **Medium Risk** | 40% - 70% | 1,994 | 42.9% |
| 🔴 **High Risk** | ≥ 70% | 784 | 91.2% |

### Sample Predictions

| CustomerID | Churn Probability | Risk Category | Actual Churn |
|------------|-------------------|---------------|--------------|
| 7590-VHVEG | 0.72 | 🔴 High Risk | No |
| 5575-GNVDE | 0.08 | 🟢 Low Risk | No |
| 3668-QPYBK | 0.85 | 🔴 High Risk | Yes |
| 9237-HQITU | 0.91 | 🔴 High Risk | Yes |
| 9305-CDSKC | 0.88 | 🔴 High Risk | Yes |

---

## 💡 Business Insights

### 🔥 Top Churn Reasons
| Factor | Churn Rate |
|--------|------------|
| 📅 Month-to-Month Contract | **42.4%** |
| 💳 Electronic Check Payment | **45.3%** |
| 🌐 Fiber Optic Internet | **41.9%** |
| 👶 New Customer (0-12 mo) | **49.4%** |
| 🛡️ No Tech Support | **41.6%** |
| 🔒 No Online Security | **41.8%** |

### 👤 High-Risk Customer Profile
- ⏱️ Average Tenure: **18.3 months**
- 💰 Average Monthly Charges: **$84.79**
- 📅 **99.2%** on Month-to-Month contracts
- 💳 **68.3%** use Electronic Check
- 🌐 **80.5%** have Fiber Optic
- 🛡️ **90.5%** have No Tech Support
- 🔒 **92.1%** have No Online Security

### 💵 Revenue Impact
| Metric | Value |
|--------|-------|
| Total Monthly Revenue | **$456,123** |
| High-Risk Monthly Revenue | **$97,458** |
| Revenue at Risk | **21.4%** |
| Potential Annual Loss | **$1,169,496** |
| Savings with 20% Churn Reduction | **$233,899** |

---

## 📁 File Structure
📦 customer-churn-prediction-ml/
├── 📄 README.md                          ← You are here
├── 📓 Customer_Churn_Analysis.ipynb      ← Main Notebook
├── 📊 WA_Fn-UseC_-Telco-Customer-Churn.csv  ← Dataset
├── 🖼️ visualizations_dashboard.png       ← Analytics Charts
├── 🖼️ model_evaluation.png              ← ML Model Charts
└── 📄 requirements.txt                   ← Dependencies




└─────────────────┘    └─────────────────┘    └─────────────────┘
