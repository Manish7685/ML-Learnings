## Notebook Summary — Week 4 Day 6

In this notebook, we focused on practical hyperparameter tuning for
Gradient Boosting models and understanding how to control overfitting.

### What was done
- Trained a default Gradient Boosting model as baseline
- Tuned key hyperparameters using GridSearchCV
- Compared tuned and default model performance
- Analyzed interaction between learning rate and number of trees
- Observed how boosting behavior changes with different parameter choices

### Key Learnings
- Gradient Boosting is highly sensitive to hyperparameters
- Lower learning rate with more trees often gives better generalization
- Tuning does not always guarantee better test accuracy
- Cross-validation optimizes validation performance, not final test performance
- Understanding parameter interactions is more important than blind search

### Final Outcome
A deeper understanding was gained of how to tune boosting models effectively
and how to interpret cases where default settings may outperform tuned models.