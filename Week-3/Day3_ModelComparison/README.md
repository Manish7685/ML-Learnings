## Notebook Summary — Week 3 Day 3

In this notebook, we learned how to compare multiple machine learning models
fairly using cross-validation instead of relying on a single test split.

### What was done
- Loaded and split the Breast Cancer dataset into training and test sets
- Defined multiple models including Logistic Regression and Decision Tree
- Evaluated each model using 5-fold cross-validation on training data
- Computed mean and standard deviation of accuracy for each model
- Created a comparison table to rank models based on performance and stability
- Selected the best model using cross-validation results
- Evaluated the selected model on the untouched test set

### Key Learnings
- Test set should not be used to compare multiple models
- Cross-validation provides a reliable estimate of model performance
- Mean accuracy reflects overall performance, while standard deviation reflects stability
- Model selection should balance both accuracy and consistency across folds

### Final Outcome
Using cross-validation, the best-performing and most stable model was selected,
and its test set performance confirmed good generalization to unseen data.