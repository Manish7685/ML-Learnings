# 🌳 Day 6 — Tree-Based Models (Decision Tree & Random Forest)

This day focuses on introducing and implementing tree-based machine learning models: **Decision Trees** and **Random Forests**.  
These models can handle nonlinear relationships and interactions naturally, making them more powerful than Logistic Regression for many problems, including the Titanic dataset.

We also compare the performance of all three models:
- Logistic Regression (Day 5)
- Decision Tree
- Random Forest

---

## 🎯 Objectives

- Train a Decision Tree classifier  
- Train a Random Forest classifier  
- Understand impurity-based feature importance  
- Evaluate both models using accuracy, precision, recall, F1, confusion matrix, ROC curve, and AUC  
- Compare all models and identify the best performer  

---

## 🧩 Steps Performed

### **1. Loaded Processed Dataset**
Imported `titanic_processed.csv` created on Day 4 after cleaning and feature engineering.

---

### **2. Train-Test Split**
Separated features (X) and target (Survived), then split into training and testing sets (80/20).

---

### **3. Decision Tree Classifier**
Trained a Decision Tree using `max_depth=4` to prevent overfitting.

Evaluated using:
- Accuracy  
- Classification report  
- Confusion matrix  
- ROC curve & AUC  

Extracted and visualized feature importance to understand which features the tree relied on.

---

### **4. Random Forest Classifier**
Trained a Random Forest with:
- `n_estimators=200`  
- `max_depth=6`  
- `random_state=42`  

This model significantly improved accuracy and AUC.

---

### **5. Feature Importance (Random Forest)**
Computed and visualized impurity-based feature importance.  
Random Forest provided more stable and reliable importance scores than a single decision tree.

---

### **6. Model Comparison**
Compared Logistic Regression, Decision Tree, and Random Forest using:

- Accuracy  
- AUC (Area Under ROC Curve)

Typical results (Titanic dataset):
- Logistic Regression → Good baseline  
- Decision Tree → Lower performance due to overfitting  
- Random Forest → Best accuracy and AUC  

Random Forest becomes the best model so far.

---

## 📊 Key Insights

- Decision Trees are intuitive but prone to overfitting  
- Random Forests improve performance by averaging multiple trees  
- Tree models handle non-linear patterns and feature interactions well  
- Random Forest achieved the highest accuracy & AUC  

---

## 📁 Files in This Directory
- Day6_Titanic_TreeModels.ipynb
- README.md

---