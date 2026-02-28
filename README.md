# 📱 Mobile Plan Recommendation (Smart vs Ultra)  
Classification Model – Megaline Customer Behavior

---

## 📖 Project Overview

This project builds a supervised learning model to recommend one of Megaline’s newer prepaid plans (Smart or Ultra) based on monthly customer behavior data (calls, minutes, messages, and internet usage).

The dataset was previously preprocessed, allowing the project to focus on model training, validation, hyperparameter tuning, and final evaluation.

---

## 🎯 Business Objective

- Predict the correct plan recommendation (Smart vs Ultra) from user behavior features  
- Maximize classification accuracy and meet a minimum target of 0.75 on the test set  
- Compare multiple algorithms and select the best-performing model  

---

## 🗂 Data

Each observation represents monthly customer behavior:

- **calls** – number of calls  
- **minutes** – total call duration (minutes)  
- **messages** – number of text messages  
- **mb_used** – internet usage (MB)  
- **is_ultra** – target label (Ultra = 1, Smart = 0)  

---

## 🛠️ Methodology

### 1️⃣ Data Split
- Training, validation, and test sets were created to support model selection and unbiased evaluation.

### 2️⃣ Model Training & Tuning
The following models were evaluated:
- Logistic Regression  
- Decision Tree Classifier (max_depth tuning)  
- Random Forest Classifier (n_estimators and max_depth tuning)  

### 3️⃣ Model Selection
The best model was selected based on validation accuracy.

---

## ✅ Results

- **Best validation model:** Random Forest  
  - n_estimators = 30, max_depth = 9  
  - validation accuracy ≈ **0.813**  

- **Final test accuracy:** ≈ **0.820**  

The target accuracy threshold (0.75) was exceeded.

---

## 🧰 Tools & Technologies

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
