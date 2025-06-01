
# Natural Language Processing 

## Domain
**Digital Content Management**

## Context

Text classification is a core task in natural language processing (NLP), especially for understanding author attributes through their writing. This project utilizes blog content to build a multi-label classifier that predicts characteristics such as age group, gender, or industry based on textual features.

---

## Dataset

**Blog Authorship Corpus**

- Contains **681,288** blog posts from **19,320** authors
- Each record includes:
  - `id`: Blogger ID
  - `gender`: Male/Female
  - `age`: Numeric
  - `topic`: Subject category of the blog
  - `sign`: Astrological sign
  - `date`: Post date
  - `text`: Blog content (main feature)

### Age Group Distribution
- Teens (13–17)
- Twenties (23–27)
- Thirties (33–47)

---

## Objective

To build a **multi-class NLP classifier** that uses blog text (`text`) to predict the topic of the blog. The project focuses on cleaning, preprocessing, and modeling using the `topic` feature as the target variable.

---

## Workflow

### 1. Data Understanding & Cleaning
- Analyzed column distributions and unique class counts
- Removed missing values and irrelevant records
- Filtered for English-only content using the `langdetect` library

### 2. Text Preprocessing
- Removed non-ASCII and special characters
- Converted all text to lowercase
- Removed stopwords and excess whitespace
- Final cleaned corpus was vectorized for modeling

### 3. Model Building
- Used `topic` as the classification target
- Vectorized text using TF-IDF or CountVectorizer
- Trained and evaluated several models:
  - Logistic Regression
  - Naive Bayes
  - Support Vector Machine (SVM)
  - Decision Tree

### 4. Evaluation Metrics
- Accuracy
- Classification Report (Precision, Recall, F1-score)
- Confusion Matrix

---

## Technologies Used

- **Python**
- **Pandas / NumPy** – Data handling
- **Scikit-learn** – ML models and metrics
- **NLTK** – Stopwords and text processing
- **Langdetect** – Language identification
- **Matplotlib / Seaborn** – Visualizations

---

## Instructions

1. Install the required libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn nltk langdetect
```

2. Run the notebook in Jupyter or JupyterLab.

3. Follow the step-by-step sections to preprocess data, train models, and evaluate results.
