# Day 3 - Exploratory Data Analysis (EDA)
This folder contains the full EDA performed on the cleaned Titanic Dataset

## Objectives
- Understand the distribution of key features.
- Analyze survival patterns
- Visualize relationships between features and the target available
- Compute survival rates across categories
- Generate ML intuition before modelling

---

## Steps Performed 
### 1. Univariate Analysis
- Age distribution
- Fare distribution
- Survival imbalance check
- Family size distribution

### 2. Bivariate Analysis
- Sex vs Survival
- Pclass vs Survival
- Age vs Survival
- Fare vs Survival
- FamilySize vs Survival

### 3. Groupby Insights
- Survival rates by Sex
- Survival rates by Pclass
- Survival rates by AgeGroup
- Survival rates by FamilySize

### 4. Correlation Heatmap
- Identified strongest predictors of survival
- Observed multicollinearity (Fare & Pclass)
- Included AgeGroup dummy variables for deeper insights

--- 

## Key Insights
- Females and 1st-class passengers had the highest survival rates
- Children survived significantly more than adults and seniors
- Higher fares strongly correlate with higher survival
- FamilySize shows non-linear behavior (alone and large families survive less)
- Sex, Pclass, Fare, and AgeGroup are the most important features for ML

---

## Files in Folder

- Day3_Titanic_EDA.ipynb - full EDA Notebook

---