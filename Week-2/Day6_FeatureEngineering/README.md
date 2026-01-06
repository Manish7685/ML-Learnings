# Week 2 · Day 6 — Feature Engineering

## Objective
Improve model performance using feature engineering **without changing the learning algorithm**, following Andrew Ng’s ML workflow.

---

## Dataset
- Breast Cancer Dataset (scikit-learn)
- Binary classification (Malignant / Benign)

---

## Baseline
- Model: Logistic Regression  
- Preprocessing: StandardScaler  
- Evaluation: Accuracy, F1 Score  

The baseline model achieved strong performance and was used as a fixed reference.

---

## Feature Engineering
Applied the following techniques:
- Interaction feature: `mean radius × mean texture`
- Log transformation: `log(mean area)`

**Result:**  
Performance metrics remained unchanged, indicating the baseline features were already highly informative.

---

## Error Analysis
Analysis of misclassified samples showed:
- Most errors were borderline cases
- Remaining errors were due to class overlap rather than missing features

---

## Key Takeaways
- Feature engineering does not always improve performance
- Strong baselines limit easy gains
- Error analysis should guide further modeling decisions

---

## Next
Week 2 · Day 7 — Cross-Validation