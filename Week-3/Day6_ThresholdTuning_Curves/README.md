### Day 6 — Threshold Tuning, ROC & Precision–Recall Curves

**Goal:**  
Understand how classification thresholds affect model behavior and learn to
evaluate models using ROC and Precision–Recall curves instead of fixed labels.

**What was done:**
- Created an imbalanced classification dataset
- Trained Logistic Regression and obtained prediction probabilities
- Plotted ROC curve and computed AUC
- Plotted Precision–Recall curve for imbalanced data analysis
- Evaluated precision, recall, and F1-score at different thresholds
- Observed trade-offs between precision and recall

**Key Learning:**  
Default probability threshold (0.5) is not always optimal. Threshold tuning
allows control over precision–recall trade-offs, and PR curves are more
informative than ROC curves for imbalanced datasets.