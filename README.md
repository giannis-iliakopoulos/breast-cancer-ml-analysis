
# Breast Cancer ML Analysis

End-to-end machine learning project for breast cancer diagnosis using the **Scikit-learn Breast Cancer dataset**.

The project explores tumor characteristics, performs exploratory data analysis (EDA), and compares multiple machine learning models to classify tumors as **malignant** or **benign**.

---

## Project Objectives

- Perform **exploratory data analysis (EDA)** on tumor features
- Visualize feature distributions and correlations
- Compare multiple machine learning models
- Evaluate performance using **accuracy, classification report, and ROC-AUC**
- Identify the **most important tumor features** influencing diagnosis

---

## Dataset

- **Source:** Scikit-learn Breast Cancer Dataset
- **Samples:** 569 tumor observations
- **Features:** 30 numerical tumor measurements including:
  - radius
  - texture
  - perimeter
  - area
  - smoothness
  - concavity
  - symmetry

Each sample is classified as:

- **Malignant**
- **Benign**

---

## Exploratory Data Analysis

EDA was performed to understand feature distributions and relationships.

Techniques used:

- Summary statistics
- Histograms
- Boxplots
- Correlation heatmap

Key observations:

- Strong correlations exist among **size-related features** (radius, perimeter, area)
- Malignant tumors tend to show **larger variation and higher values**
- Some overlap exists, meaning **multiple features are required for accurate classification**

---

## Data Preparation

- Dataset split into **80% training** and **20% testing**
- **Stratified sampling** used to preserve class balance
- **StandardScaler** applied to normalize feature ranges

---

## Model Development

Three models were compared using **5-fold cross-validation**:

| Model | Mean Accuracy |
|------|------|
| Logistic Regression | **0.9807** |
| Random Forest | 0.9614 |
| SVM (RBF) | 0.9122 |

**Best Model:** Logistic Regression  
Chosen due to **highest accuracy and most stable performance**.

---

## Final Model Evaluation

Test set results:

- **Accuracy:** 98.25%

Classification performance:

| Class | Precision | Recall | F1 Score |
|------|------|------|------|
| Malignant | 0.98 | 0.98 | 0.98 |
| Benign | 0.99 | 0.99 | 0.99 |

The model demonstrates **strong and balanced classification performance** across both tumor types.

---

## ROC Curve Analysis

- **ROC-AUC Score:** ~0.995
- The curve remains near the **top-left corner**, indicating excellent discrimination between malignant and benign tumors.

---

## Feature Importance

Using Logistic Regression coefficients, the most influential tumor characteristics include:

- Worst texture
- Radius error
- Worst concave points
- Worst area
- Worst radius
- Worst symmetry
- Area error
- Worst concavity
- Worst perimeter
- Worst smoothness

These features strongly contribute to diagnosis predictions.

---

## Conclusion

Logistic Regression provides **excellent and reliable performance** for breast cancer classification.

Tumor **size, shape, and concavity-related measurements** appear to be the strongest indicators of malignancy.

The model demonstrates strong potential for **supporting diagnostic decision-making systems** in medical data analysis.

---

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## Author

**Giannis Iliakopoulos**
