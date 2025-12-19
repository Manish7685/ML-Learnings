# 📘 Day 5 — Logistic Regression Modeling (Titanic Dataset)

This session marks the first complete machine learning pipeline in the Titanic survival prediction project.  
We used Logistic Regression to model binary survival outcomes using the ML-ready dataset created in Day 4.

---

## 🎯 Objectives

- Build a logistic regression classifier  
- Scale numerical features  
- Train the model using the training set  
- Evaluate using standard classification metrics  
- Plot ROC curve and compute AUC  
- Interpret feature coefficients  

---

## 🧩 Steps Performed

### **1. Load Processed Dataset**
Imported `titanic_processed.csv`, checked structure, and verified clean numeric data.

---

### **2. Train-Test Split**
Separated features and target, then performed an 80-20 split.

---

### **3. Feature Scaling**
Applied **StandardScaler** to normalize feature ranges and ensure stable logistic regression training.

---

### **4. Model Training**
Trained a `LogisticRegression(max_iter=1000)` model on the scaled training data.

---

### **5. Model Evaluation**
Computed:

- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion matrix (with visualization)  
- ROC Curve  
- AUC score  

---

### **6. Feature Importance**
Extracted and visualized logistic regression coefficients to understand which factors influenced survival.

---

## 📊 Key Insights

- The model achieved strong accuracy and balanced precision/recall  
- ROC-AUC score shows good separability between survivors and non-survivors  
- Important positive predictors included **Sex (female)**, **Fare**, and **AgeGroup features**  
- Negative predictors included **Pclass**, **IsAlone**, and **Fare_Log**  

---

## 📁 Files in This Directory

- Day5_Titanic_LogisticRegression.ipynb
- README.md

---