# Credit Card Fraud Detection System

## 📌 Problem Statement

Fraudulent transactions pose a significant risk to financial institutions, leading to substantial monetary losses.
The goal of this project is to build a machine learning model that can accurately detect fraudulent transactions while minimizing false negatives.

---

## 📊 Dataset

* Credit Card Fraud Detection Dataset (Kaggle)
* ~284,000 transactions
* Highly imbalanced dataset:

  * 0 → Normal transactions
  * 1 → Fraudulent transactions (~0.17%)

---

## ⚙️ Project Workflow

### 1. Data Understanding & Exploration

* Analyzed class distribution and identified extreme imbalance
* Visualized fraud vs non-fraud transactions

### 2. Data Preprocessing

* Scaled `Amount` feature using **StandardScaler**
* Removed irrelevant feature (`Time`)

### 3. Handling Class Imbalance

* Applied **SMOTE (Synthetic Minority Oversampling Technique)**
* Balanced minority (fraud) and majority classes

### 4. Model Building

Trained and compared multiple models:

* Logistic Regression
* Random Forest
* LightGBM

---

## 📈 Model Evaluation

* Used **AUC-ROC** as a general performance metric
* Focused on:

  * **Recall** (to minimize missed fraud cases)
  * Precision and F1-score
  * Confusion Matrix

👉 **Best Model:** Logistic Regression
👉 **AUC Score:** ~0.97

---

## 🔍 Key Insights

* Dataset is highly imbalanced, requiring special handling
* Logistic Regression performed strongly due to PCA-transformed features
* Recall is the most critical metric in fraud detection
* SMOTE significantly improved detection of fraudulent transactions

---

## 💡 Business Impact

* Enables early detection of fraudulent transactions
* Reduces financial losses for organizations
* Improves risk management and decision-making

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* LightGBM
* Imbalanced-learn (SMOTE)

---

## 🚀 Conclusion

This project demonstrates how machine learning can be effectively used to detect fraudulent financial transactions by handling class imbalance and focusing on critical evaluation metrics like recall, ensuring practical and real-world applicability.

---
