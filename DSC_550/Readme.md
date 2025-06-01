
# Credit Risk Modeling - Data Selection ,  EDA. Classifcation modelling and Evaluation

## Author
**Saravanan Janarthanan**


## Project Overview

This term project focuses on **credit risk modeling**, a critical area in financial data mining. The objective is to analyze a real-world dataset to understand patterns that may influence loan defaults, supporting better decision-making in lending.

The milestone includes:
- Defining the business problem
- Selecting and exploring a dataset
- Creating visualizations to understand feature relationships
- Beginning the groundwork for a predictive model

---

## Business Problem

Financial institutions must evaluate the risk of loan applicants defaulting on payments. This project aims to build a model that helps identify high-risk borrowers based on key financial and demographic indicators.

The **target variable** for this analysis is `loan_status`, indicating whether a loan has defaulted (`1`) or not (`0`).

---

## Dataset

The dataset includes various features that may affect loan approval and default rates, such as:
- `person_age`: Applicant's age
- `person_income`: Monthly income
- `loan_amnt`: Loan amount
- `loan_int_rate`: Interest rate
- `loan_intent`: Purpose of the loan
- `person_home_ownership`: Type of home ownership
- `cb_person_cred_hist_length`: Credit history length
- `cb_person_default_on_file`: Past default history

---

## Exploratory Data Analysis (EDA)

The following visualizations were created:
- **Histogram of Age**: To analyze distribution and detect any skewness
- **Pie Chart of Loan Status**: To visualize the proportion of default vs non-default loans
- **Income Distribution**: To understand how income varies among applicants
- **Loan Amount vs Default Status**: To detect patterns or thresholds linked to defaults

Insights drawn from these visualizations begin to form hypotheses about what drives loan defaults.

---

## Conclusions
Based on training models the  findings from  the best optinal model among the 4 is listed below 

=============================================================================================================================
*        Model Name         * Accuracy  * Precision *  Recall   * F1 Score  * True Pos  * True Neg  * False Pos * False Neg *
=============================================================================================================================
* Logsitic Regression       *      0.81 *      0.56 *      0.77 *      0.65 *      1128 *      4197 *       329 *       858 *
* Support Vector Machine    *      0.86 *      0.69 *      0.74 *      0.71 *      1081 *      4571 *       376 *       484 *
* Random Forest Classifier  *      0.91 *      0.83 *      0.75 *      0.79 *      1099 *      4842 *       358 *       213 *
* XGBooster Classifier      *      0.92 *      0.90 *      0.73 *      0.80 *      1071 *      4938 *       386 *       117 *
============================================================================================================================= 

Evaluation Metrics

The following metrics are chosen for evaluating the performance of classification models due to their ability to provide comprehensive insights:

- Accuracy: Measures the ratio of correctly predicted instances to the total instances. This metric gives a quick snapshot of the model's overall performance across all classes.

- Precision: Represents the ratio of correctly predicted positive observations to the total predicted positives. Precision is crucial when the cost of false positives is high. For example, in spam detection, high precision ensures that fewer legitimate emails are incorrectly marked as spam.

- Recall: Indicates the ratio of correctly predicted positive observations to all observations in the actual positive class. Recall is essential when the cost of false negatives is high. For instance, in disease screening, high recall ensures that most actual positive cases are identified, reducing the risk of missing true positive cases.

- F1 Score: The harmonic mean of precision and recall. The F1 score balances both precision and recall, making it useful as a single metric for evaluating model performance, particularly in cases of class imbalance.

- Confusion Matrix: A table that describes the performance of a classification model by displaying the true positives (TP), true negatives (TN), false positives (FP), and false negatives (FN). The confusion matrix provides detailed insights into the model's performance, helping to diagnose specific issues, such as whether the model is more prone to false positives or false negatives.

These metrics collectively offer a well-rounded evaluation of a model's performance, highlighting different aspects and helping to identify areas for improvement.

Based on the evaluation metrics, the XGBoost Classifier excels in several aspects:

- Accuracy: The XGBoost Classifier has a high accuracy of 92%, indicating that it correctly predicted 92% of the test values. The Random Forest Classifier is close behind with 91% accuracy.
- Precision: With a precision of 90%, the XGBoost Classifier demonstrates that it correctly identified 90% of the positive predictions, effectively reducing the false positive rate..
- Recall: The recall score for XGBoost is 73%, which is lower than the optimal standard and slightly less than Logistic Regression's recall of 77%. This indicates that while XGBoost has a higher false negative rate, it is still competitive.
- F1 Score: The F1 score, balancing precision and recall, is 80% for XGBoost, higher than the other models, suggesting it better identifies positive cases.
- Confusion Matrix: The confusion matrix shows that the XGBoost Classifier has higher true positive and true negative predictions compared to other models, indicating better overall prediction capability.
- In conclusion, the XGBoost Classifier outperforms other optimized models, demonstrating superior accuracy, precision, and balanced performance.
- The comprehensive evaluation indicates that the XGBoost Classifier is the most optimized model for this classification task, providing the best balance among accuracy, precision, recall, and F1 score. Its ability to effectively handle class imbalances and minimize both false positives and false negatives makes it the preferred choice. However, the Random Forest Classifier is also a strong performer, with metrics only slightly lower than XGBoost. Support Vector Machine and Logistic Regression are suitable for specific scenarios where their particular strengths (higher recall for Logistic Regression and balanced performance for SVM) are advantageous.

Overall, selecting the right model depends on the specific needs of the application, whether prioritizing reducing false positives, minimizing false negatives, or balancing both effectively.

Project Learning
This project provides a comprehensive understanding of developing a business solution using data science and machine learning. It encompasses various critical stages, including:

- Data Cleaning: Preparing raw data by handling missing values, correcting inconsistencies, and removing noise.
- Data Transformation: Modifying data formats and types to suit analytical needs.
- Data Analysis: Exploring and interpreting data to identify patterns and insights.
- Feature Engineering: Creating new features or modifying existing ones to improve model performance.
- Standardizing the Data: Ensuring that data is on a comparable scale.
- Balancing the Data: Addressing class imbalances to prevent biased model outcomes.
- Building and Training the Model: Developing and fitting the model to the training data.
- Evaluating the Model: Assessing model performance using various metrics.
- The project also delves into hyperparameter tuning, understanding computational constraints, and fine-tuning to ensure the model's performance is not significantly impacted by infrastructure limitations. This holistic approach enhances the ability to develop and deploy robust machine learning models in real-world business applications.

## Technologies Used

- **Python**
- **Pandas** and **NumPy** for data handling
- **Matplotlib** and **Seaborn** for visualizations
- **Jupyter Notebook** for iterative analysis

---

## Next Steps

In future milestones, the project will:
- Perform further feature engineering
- Recommend actions for risk mitigation

---

## Instructions

1. Clone this repository or download the notebook.
2. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn
```
3. Open the notebook in Jupyter and run all cells sequentially.
