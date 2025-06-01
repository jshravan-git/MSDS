
# Predictive Analytics – Airline customer Satisfaction prediction

## Author
**Saravanan Janarthanan**

## Project Overview

This notebook focuses on the pre-processing, model building, and interpretation of predictions. The dataset consists of training and test datasets provided separately, allowing the implementation of supervised machine learning pipelines.

---

## Objectives

- Analyze and clean the dataset
- Encode categorical variables
- Develop and evaluate predictive models
- Interpret model results to draw meaningful conclusions

---

## Key Questions Addressed

- Is the data sufficient to answer the research questions?
- Are any visualizations necessary for better understanding?
- Should the model or its evaluation strategy be revised?
- Are the initial expectations still realistic based on model outcomes?

---

## Data Preparation

- **Missing values** handled and irrelevant columns (e.g., `id`, `SN`) dropped.
- **Categorical columns** encoded using ordinal encoding.
- **Training and test datasets** were cleaned and preprocessed using consistent methods to ensure compatibility during model evaluation.

---

## Modeling

Several models were trained and evaluated:
- **Decision Tree Classifier**
- **Random Forest Classifier**
- **Logistic Regression**
- **Gradient Boosting**
- **XGBoost Classifier**

### Evaluation Metrics:
- Accuracy
- Classification report (Precision, Recall, F1-score)
- Feature importance plots

---

## Insights

- **XGBoost** and **Random Forest** performed well on accuracy and recall.
- Feature importance helped identify key drivers for the prediction outcome.
- Data encoding and consistent preprocessing between train/test sets were critical for valid results.

---

## Summary
- Best Overall Performance: XGBoost Optimized and Random Forest due to their balanced metrics and low false negative rates.
- Most Efficient in Reducing False Positives: Neural Network with a lower false positive count.
- Simple and Fast Option: Logistic Regression is not competitive in performance but could serve as a quick reference point.
- Trade-offs in Complexity and Interpretability: Models like Decision Trees and Random Forest provide interpretability through feature importance, while Neural Networks and SVM offer flexibility for more complex decision-making.
- In summary, XGBoost Optimized is the most suitable choice for applications requiring the highest precision and recall balance, while Random Forest and SVM provide comparable alternatives.

---
## Technologies Used

- **Python**
- **Pandas / NumPy**
- **Scikit-learn**
- **Matplotlib / Seaborn**
- **XGBoost**

---

## Instructions

1. Download or clone the repository.
2. Install dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn xgboost
```
3. Run the notebook in Jupyter or JupyterLab.
