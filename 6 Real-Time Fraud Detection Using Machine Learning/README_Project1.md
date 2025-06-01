
# Real-Time Fraud Detection Using Machine Learning

This Jupyter notebook that demonstrates how to build a real-time fraud detection system using machine learning techniques. 

---

## Objective

To develop a machine learning-based system to identify and prevent fraudulent banking transactions in real time, enhancing security and minimizing financial losses.

---

## Dataset Summary

- **Records**: 200,000 banking transactions
- **Features**: 24 columns including customer info, transaction details, and fraud indicators
- **No missing values or duplicates**

---

##  Data Preprocessing

- Dropped irrelevant or sensitive fields (e.g., names, emails)
- Created engineered features:
  - `Transaction_Hour`
  - `Amt_to_Balance_Ratio`
  - `Is_Night`
  - `High_Value_Transaction`
  - `Device_Location_Mismatch`
  - `Customer_Txn_Count`

---

##  Exploratory Data Analysis (EDA)

- Univariate analysis on age, gender, account type, and balance
- Multivariate insights showed no strong pattern tied to any single feature
- Peak fraud activity between 10 PM and 6 AM
- Weak correlation between numerical features and fraud
---

##  Visualizations

The notebook includes several visualizations to support analysis and model insights:

- **Distribution Plots**: Age, transaction amount, and account balance distributions for both fraud and non-fraud cases
- **Box Plots**: Comparison of transaction characteristics across fraud labels
- **Fraud by Hour**: Time-based trends showing higher fraud activity during late-night hours (10 PM – 6 AM)
- **Categorical Analysis**: Multivariate breakdowns by gender, account type, device type, and transaction type
- **Correlation Heatmaps**: Visual display of relationships (or lack thereof) between numerical variables and fraud

These visualizations helped guide feature engineering and informed model selection.

---

##  Machine Learning Models Used

- Logistic Regression
- Random Forest
- XGBoost
- Neural Network

### Evaluation Metrics:
- Precision
- Recall
- F1-Score
- 10-Fold Cross Validation

---

##  Class Imbalance Handling

Used **SMOTE (Synthetic Minority Over-sampling Technique)** to balance the dataset (originally only 5% fraudulent cases).

---

##  Key Findings

- **Neural Network** had the best recall (caught most fraud)
- **XGBoost** had the best precision (fewer false alarms)
- **Random Forest** offered consistent all-around performance

---

##  Recommendations

- Use Neural Network to maximize fraud detection
- Use XGBoost to minimize false positives
- Combine models (ensemble) for balanced performance

---

## 📁 File Contents

- `Saravanan_Janarthanan_DSC680_Project_1_MLS2_supporting.ipynb` – Full project notebook

---


