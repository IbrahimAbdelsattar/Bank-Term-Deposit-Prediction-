# 🏦 Bank Term Deposit Prediction

## 📋 Project Overview
This project focuses on predicting whether a customer will subscribe to a term deposit product based on their personal, financial, and campaign-related information. Using machine learning models, we aim to help banks **optimize marketing strategies**, **improve targeting**, and **increase customer conversion rates**.

---

## 🎯 Project Objectives
- Perform **Exploratory Data Analysis (EDA)** to understand customer demographics and campaign characteristics.
- Preprocess the data by **handling missing values**, **encoding categorical features**, and **scaling**.
- Apply and evaluate multiple **classification models**.
- Select the best-performing model based on key evaluation metrics.
- Provide **business insights** and recommendations.

---

## 📦 Dataset Information
- **Source**: [Kaggle - Bank Marketing Dataset](/kaggle/input/data-of-customers/train.csv)
- **Records**: 45,211 entries
- **Features**: 17 input variables + 1 target variable

### Main Features:
- **Personal attributes**: `age`, `job`, `marital`, `education`, `default`, `housing`, `loan`
- **Campaign attributes**: `contact`, `month`, `day_of_week`, `duration`
- **Historical campaign data**: `pdays`, `previous`, `poutcome`
- **Economic context**: `emp.var.rate`, `cons.price.idx`, `cons.conf.idx`, `euribor3m`, `nr.employed`
- **Target**: `y` — Whether the client subscribed to a term deposit (`yes` or `no`).

---

## 🛠️ Project Workflow

### 1. Exploratory Data Analysis (EDA)
- Statistical summaries
- Visualizations (bar plots, histograms, correlation heatmaps)
- Outlier detection and treatment

### 2. Data Preprocessing
- Encoding categorical variables (Label Encoding / One-Hot Encoding)
- Feature scaling with **StandardScaler**
- Addressing class imbalance using techniques like **SMOTE** if necessary

### 3. Model Building
- **Logistic Regression**
- **Decision Tree Classifier**
- **Random Forest Classifier**
- **Gradient Boosting Classifier**
- **XGBoost Classifier**

### 4. Model Evaluation
- Accuracy, Precision, Recall, F1-Score
- ROC-AUC Curve
- Confusion Matrix Analysis

### 5. Model Selection
- Compare performance across models
- Choose the best model based on balanced metrics

---

## 📊 Results
- Best-performing model: **Random Forest Classifier** (example)
- Achieved high **precision** and **recall** in predicting potential term deposit subscribers.
- Important features influencing prediction:
  - `duration`
  - `previous outcomes`
  - `pdays`
  - `contact type`
  - `employment variation rate`

---

## 💡 Business Implications
- Campaign strategies can be **better focused** on customers with higher predicted probabilities of subscribing.
- **Optimize resource allocation** by reducing calls to low-probability customers.
- **Targeted marketing** based on insights can significantly improve overall success rates.

---

## 📚 Conclusion
By building predictive models, banks can gain a **data-driven understanding** of customer behavior, **improve marketing efficiency**, and **maximize term deposit subscriptions**.

---

## 🚀 Future Work
- Hyperparameter tuning with **GridSearchCV** or **RandomizedSearchCV**.
- Deploy the model using **Flask API** or **Streamlit** for real-time predictions.
- Further exploration of **deep learning models** for more complex patterns.

---
