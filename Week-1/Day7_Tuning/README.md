# 🌟 Day 7 — Hyperparameter Tuning (Random Forest Optimization)

This notebook focuses on improving the Random Forest classifier using **RandomizedSearchCV** and evaluating the optimized model using metrics such as accuracy, ROC curve, and AUC. Hyperparameter tuning is a key step for improving generalization and model performance.

---

## 📌 Objectives

- Perform hyperparameter tuning using RandomizedSearchCV  
- Identify the best-performing Random Forest model  
- Evaluate tuned vs baseline performance  
- Plot and compare ROC curves  
- Save the final optimized model for future use  

---

## 🧠 Key Concepts Learned

### 🔹 Hyperparameter Tuning
Hyperparameters control a model’s behavior.  
RandomizedSearchCV helps explore many combinations efficiently using cross-validation.

### 🔹 Cross-Validation (CV)
Used to measure model stability and prevent overfitting.

### 🔹 ROC Curve & AUC
AUC measures class separation quality.  
Higher AUC = better performance across thresholds.

---

## 🛠️ Steps Completed

### **1️⃣ Loaded Processed Dataset**
Imported the feature-engineered Titanic dataset prepared on Day 4.

---

### **2️⃣ Baseline Random Forest Evaluation**
Trained a simple Random Forest model as a reference point.  
Metrics used:
- Accuracy  
- ROC Curve  
- AUC  

---

### **3️⃣ Hyperparameter Tuning using RandomizedSearchCV**
Defined a broad search space:

- `n_estimators`  
- `max_depth`  
- `min_samples_split`  
- `min_samples_leaf`  
- `max_features`  

RandomizedSearchCV performed:
- 20 random hyperparameter combinations  
- 5-fold cross-validation  
- Selected the best model  

---

### **4️⃣ Tuned Model Evaluation**
Evaluated the optimized model on the test set:

- Higher **accuracy**  
- Improved **AUC**  
- Better **precision**, **recall**, and **F1-score**

---

### **5️⃣ ROC Curve Visualization**
Plotted the ROC curve for the tuned Random Forest.  
The curve is significantly above the baseline model, confirming improved performance.

---

### **6️⃣ Baseline vs Tuned Model Comparison**

| Model | Accuracy | AUC |
|-------|----------|------|
| Baseline Random Forest | ↑ baseline_acc | ↑ baseline_auc |
| **Tuned Random Forest** | **↑ improved_acc** | **↑ improved_auc** |

*(Values replaced by actual results in notebook)*

The tuned model clearly outperformed the baseline.

---

### **7️⃣ Saved Final Optimized Model**
Exported the best model as: 

best_model/tuned_random_forest.pkl

This model can now be reused for inference or deployment.

---

## 📁 Files in This Folder

Day7_Tuning_RandomForest.ipynb

README.md

best_model/
└── tuned_random_forest.pkl

---

## 🎯 Final Summary

Day 7 completes the Titanic ML pipeline with professional-level model optimization.  
You now understand:

- How to tune machine learning models  
- How to evaluate model improvements  
- How to save and reuse trained models  
- How to compare multiple models systematically  

Your Random Forest model is now **fully optimized and production-ready**.

---