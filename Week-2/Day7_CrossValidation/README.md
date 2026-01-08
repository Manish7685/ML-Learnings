### Day 7 — Cross-Validation & Model Stability (Breast Cancer Dataset)

**Goal:**  
Learn how to evaluate models reliably using k-fold cross-validation and avoid
overfitting to the test set.

**What was done:**
- Created a hold-out test set before model selection
- Applied feature scaling using StandardScaler
- Compared Logistic Regression models using 5-fold cross-validation
- Evaluated mean accuracy and stability (standard deviation)
- Selected best model and tested on unseen test set

**Key Learning:**
Model selection must be done using cross-validation on training data, and the
test set should be used only once for final performance estimation.