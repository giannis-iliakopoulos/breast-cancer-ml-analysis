# Breast Cancer ML Analysis

End-to-end machine learning project for breast cancer diagnosis using the sklearn dataset.

## Project Goals
- Classify tumors as malignant vs benign
- Compare multiple ML models
- Evaluate performance with ROC-AUC and cross-validation

## Methods
- Exploratory Data Analysis (EDA)
- Feature visualization & correlation analysis
- Train/test split (80/20, stratified)
- Standardization (StandardScaler)
- Models:
  - Logistic Regression
  - Support Vector Machine (RBF)
  - Random Forest
- 5-fold Cross-Validation
## Results
- Best model: Logistic Regression
- Test Accuracy: ~98%
- Tumor size and shape features are strong indicators, though size alone is insufficient.

## Tools
Python, NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn
