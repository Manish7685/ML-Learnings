## Notebook Summary — Week 4 Day 4

In this notebook, we focused on understanding and comparing different methods
for interpreting tree-based models.

### What was done
- Trained a Random Forest model on the Breast Cancer dataset
- Verified model performance before interpretation
- Extracted built-in feature importance from Random Forest
- Computed permutation importance using the test set
- Compared built-in and permutation importance side-by-side

### Key Learnings
- Built-in feature importance can be biased toward certain features
- Permutation importance is model-agnostic and based on prediction performance
- Features important for splits are not always the same as features important
  for predictions
- Reliable model interpretation requires multiple explanation methods

### Final Outcome
Permutation importance provided more trustworthy feature rankings, improving
confidence in model explanations and making the Random Forest model more
interpretable for real-world use.