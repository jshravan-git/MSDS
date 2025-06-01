
# NLP Chatbot for Industrial Safety – Capstone Project


## Domain
**Industrial Safety using NLP**

## Problem Statement

Despite safety protocols, employees in industrial environments continue to experience serious accidents. This project aims to build a **chatbot using NLP and machine learning** that interprets accident descriptions and identifies critical safety risks to aid in proactive risk management.

---

## Dataset

Sourced from Kaggle: [Industrial Safety and Health Analytics Database](https://www.kaggle.com/ihmstefanini/industrial-safety-and-health-analytics-database)

### Features

- `Data`: Date/time of incident
- `Countries`: Country where incident occurred
- `Local`: City of the plant
- `Industry Sector`: Manufacturing sector
- `Accident Level`: Severity from I (low) to VI (very high)
- `Potential Accident Level`: Hypothetical severity
- `Genre`: Gender of the individual
- `Employee or Third Party`: Injured person's role
- `Critical Risk`: Risk factor involved
- `Description`: **Free-text narrative** of the incident

---

## Objective

Build an **ML/DL-based chatbot** that analyzes the free-text `Description` field and classifies:
- Critical risk type
- Severity level
- Other safety attributes (optional)

This utility can help **EHS professionals** assess incidents faster and prioritize safety responses.

---

## Methodology

### Data Preparation
- Loaded 425 rows × 11 columns
- Cleaned and renamed columns
- Verified absence of missing values
- Focused on `Description` as the key NLP feature

### NLP Preprocessing
- Removed special characters and stopwords
- Converted text to lowercase
- Tokenization and vectorization (TF-IDF)

### Modeling Approaches
- **Multi-class classification** to predict:
  - `Critical Risk`
  - `Accident Level`
- ML algorithms used:
  - Logistic Regression
  - SVM
  - Random Forest
- Evaluation:
  - Accuracy, Precision, Recall, F1-Score

### Chatbot Integration
- Designed a text-based prototype interface
- Takes user input and returns the predicted safety risk class

---

## Technologies Used

- **Python**
- **Pandas / NumPy** – Data analysis
- **NLTK / Scikit-learn** – NLP and ML
- **Streamlit or Flask (optional)** – Chatbot interface
- **Matplotlib / Seaborn** – Data visualization

---

## Instructions

1. Install dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn nltk
```

2. Download the dataset from Kaggle if not included.

3. Run the notebook or deploy the chatbot using a web interface like Streamlit.
