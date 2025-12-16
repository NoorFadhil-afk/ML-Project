<div align="center">

# 💳 **Credit Card Fraud Detection**

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![ML](https://img.shields.io/badge/Machine%20Learning-Fraud%20Detection-purple)
![Status](https://img.shields.io/badge/Project-Completed-success)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

*A Machine Learning project to detect fraudulent credit card transactions using imbalanced data techniques and multiple classification models.*

</div>

---

## 🎯 Project Objectives

* 🔍 Detect fraudulent transactions with **high recall** (catch as many fraud cases as possible)
* ⚖️ Handle **highly imbalanced datasets** effectively
* 🤖 Compare multiple ML models:

  * KNN
  * Logistic Regression
  * Random Forest
* 📊 Evaluate models using standard and fraud-focused metrics

---

## 📂 Dataset Information

* **Source:** Kaggle – Credit Card Fraud Detection Dataset
* **Total Transactions:** 284,807
* **Fraud Cases:** 492 (Highly Imbalanced)
* **Features (30):**

  * `V1 – V28` (PCA-transformed)
  * `Time`
  * `Amount`
* **Target Variable:**

  * `Class` → 0 = Normal, 1 = Fraud

---

## 🛠 Data Preprocessing

✔ Remove missing or corrupted values
✔ Feature Scaling using **StandardScaler**
✔ Create new features:

* `scaled_Time`
* `scaled_Amount`

✔ Train-Test Split:

* 🧪 80% Training
* 🔬 20% Testing

✔ Handle class imbalance using:

* SMOTE
* Oversampling / Undersampling
* Class Weights

---

## 🧠 Features Used

* Time
* Amount
* V1 – V28
* Engineered features:

  * `scaled_Time`
  * `scaled_Amount`

> Features are removed **only if correlation analysis shows no importance**.

---

## 🤖 Models Implemented

### Required Models

* K-Nearest Neighbors (KNN)
* Logistic Regression
* Random Forest

### Training Strategy

* Hyperparameter tuning using **GridSearchCV**
* **5-Fold Cross-Validation**
* Performance comparison across models

---

## 📈 Model Evaluation

Each model is evaluated using:

* Accuracy
* Precision
* **Recall (Critical for Fraud Detection)**
* F1-score
* Confusion Matrix
* ROC Curve
* AUC Score

### 🚨 Fraud Detection Priority

* **High Recall for Fraud (Class 1)** is mandatory
* Lower precision is acceptable if recall improves

---

## 📊 Outputs & Visualizations

* ✅ Fraud Predictions (0 / 1)
* 📄 Classification Report
* 📉 Visualizations:

  * Correlation Heatmap
  * Fraud vs Valid Transaction Count
  * ROC Curve
  * Confusion Matrix
  * Feature Importance (Random Forest)

---

## ⚙️ System Requirements

* **Python:** 3.8+
* **Libraries:**

  * pandas
  * numpy
  * scikit-learn
  * matplotlib
  * seaborn
  * imblearn (SMOTE)
* **Environment:**

  * Jupyter Notebook / Google Colab

---

## ⚠️ Project Constraints

* Highly imbalanced dataset
* PCA-transformed features (limited interpretability)
* Rare fraud cases → risk of overfitting

---

## ✅ Success Criteria

* 🔹 **Recall (Fraud):** > 80%
* 🔹 **F1-score (Fraud):** > 0.70
* 🔹 **AUC Score:** > 0.90

---

## 👩‍💻 Author

**Noor Ali Fadel**
Bachelor’s Degree in Internet & Cybersecurity
Machine Learning & Fraud Detection Project

---

⭐ *If you like this project, don’t forget to star the repository!*
