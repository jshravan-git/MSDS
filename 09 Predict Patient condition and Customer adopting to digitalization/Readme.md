
# Supervised Learning Project – Medical Research

## Domain
**Medical Research**

## Context

A medical research university is analyzing biomechanical data to predict patient conditions. The data has been anonymized due to confidentiality. The university’s internal AI team is tasked with building a supervised learning model to predict the condition of a patient based on test results.

---

## Dataset Description

The dataset includes **three CSV files** representing different patient groups:

- **Normal.csv** – Patients with normal biomechanical features
- **Type_H.csv** – Patients with one specific condition
- **Type_S.csv** – Patients with another condition

Each record includes **six biomechanical features** extracted from patient body part orientations.

---

## Objectives

- Load and explore the structure of all datasets
- Combine data and generate target labels
- Perform preprocessing and feature scaling
- Train and evaluate multiple supervised learning models
- Compare results and select the best-performing model

---

## Methodology

### Part A: Data Understanding
- Loaded all CSV files using `pandas`
- Compared shapes and column names
- Merged all datasets with appropriate class labels

### Part B: Model Building
Applied the following classification algorithms:

- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **Support Vector Machine (SVM)**
- **Naive Bayes**
- **Decision Tree**
- **Random Forest**

### Evaluation Metrics:
- Accuracy
- Confusion Matrix
- Cross-validation scores

---

## Key Insights

- Feature similarity was observed across datasets with differences in values, not structure
- Models like **Random Forest** and **SVM** achieved higher accuracy
- Proper labeling and preprocessing significantly impacted performance

---

## Technologies Used

- **Python**
- **Pandas / NumPy** – Data manipulation
- **Matplotlib / Seaborn** – Visualization
- **Scikit-learn** – Machine Learning models

---

## Instructions

1. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

2. Open the notebook in Jupyter or JupyterLab.

3. Execute cells in order to reproduce the analysis and model training.
