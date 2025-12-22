# Week 2 Day 1 — California Housing Linear Regression

This notebook implements Linear Regression on the **California Housing Dataset**, using both:

- Scikit-Learn’s `LinearRegression`
- Manual Gradient Descent (multivariate)

The goal is to understand real-world regression workflows and compare GD with sklearn.

---

## 🔹 Concepts Covered
- Linear Regression using Andrew Ng notation:  
  \[
  f_{w,b}(x) = w x + b
  \]
- Cost function  
  \[
  J(w,b) = \frac{1}{2m}\sum (f_{w,b}(x^{(i)}) - y^{(i)})^2
  \]
- Train/Test split  
- Model training with sklearn  
- Evaluation: MAE, MSE, R²  
- Implementing Gradient Descent with feature scaling  
- Comparing GD weights vs sklearn weights  
- Plotting True vs Predicted values  
- Cost convergence curve

---

## 🔹 Steps Performed
1. Loaded California Housing dataset (`fetch_california_housing`).
2. Split into training and test sets.
3. Trained Linear Regression using sklearn.
4. Evaluated model performance.
5. Implemented multivariate Gradient Descent:
   - Standardized features  
   - Updated weights and bias over iterations  
6. Plotted cost reduction.
7. Compared sklearn and GD parameters.

---

## 🔹 Results
- Gradient Descent converges when features are scaled.
- Sklearn and GD weights are close.
- R² score ~0.60–0.65 (normal for this dataset).

---

## 🔹 Files
Week-2/

└── Day1_California_Housing_Linear_Regression.ipynb

└── README.md
---

## ✔ Summary
A complete ML regression pipeline was built using real data, covering both the analytical and optimization-based approaches to Linear Regression.