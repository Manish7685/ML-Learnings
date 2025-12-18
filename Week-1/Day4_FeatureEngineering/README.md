# Day 4 – Feature Engineering & ML Preparation (Titanic Dataset)

This notebook focuses on transforming the cleaned Titanic dataset into a fully machine-learning–ready dataset.  
We use insights from Day 3 (EDA) to engineer new features, encode categorical variables, and prepare the data for model training in future sessions.

---

## 🎯 Objectives

- Load the cleaned dataset created on Day 2  
- Recreate and encode the `AgeGroup` feature  
- Engineer new meaningful features  
- Drop irrelevant or redundant columns  
- Validate the dataset  
- Perform a train–test split  
- Save the final processed dataset for Day 5  

---

## 🧩 Steps Performed

### 1. **Load Cleaned Dataset**
Imported `titanic_cleaned.csv` from Day 2 and verified data types, missing values, and structure.

---

### 2. **Recreate & Encode AgeGroup**
`AgeGroup` (Child, Teen, Adult, Middle-aged, Senior) was created again because it was not saved earlier.

Applied one-hot encoding to generate:
- `AgeGroup_Teen`
- `AgeGroup_Adult`
- `AgeGroup_Middle-aged`
- `AgeGroup_Senior`

These new columns were converted into numeric dummy variables.

---

### 3. **Feature Engineering**
Several additional features were created to capture deeper patterns in survival:

#### 🔹 **Fare_Log**
Applied log transformation:
- Reduces right-skewed distribution of Fare  
- Helps linear models train more effectively

#### 🔹 **AgeBin**
Converted Age into demographic bins:
- Child (0), Teen (1), Adult (2), Middle-aged (3), Senior (4)

Captures non-linear survival patterns.

#### 🔹 **IsAlone**
Derived from the `FamilySize` feature:
- `1` → passenger traveling alone  
- `0` → passenger traveling with family  

This is a powerful predictor in Titanic ML models.

---

### 4. **Dropped Irrelevant Columns**
Removed columns that do not provide predictive value:
- `SibSp`
- `Parch`

These columns are identifiers or unstructured text and do not help the model.

---

### 5. **Dataset Validation**
Verified:
- No missing values  
- All columns are numeric  
- Engineered features exist  
- Dataset shape is correct  
- No redundant or duplicate columns  

---

### 6. **Train–Test Split**
Used an 80-20 split:

```python
train_test_split(X, y, test_size=0.2, random_state=42)