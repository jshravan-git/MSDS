
# Recommendation Systems Project – Saravanan Janarthanan

## Domain
**Smartphones / Electronics**

## Context

India is one of the largest markets for smartphones, with hundreds of millions of users generating large volumes of product feedback. Understanding consumer behavior and preferences through ratings and reviews enables businesses to recommend products that better match user expectations. This project builds a recommendation system to suggest smartphones based on user behavior and popularity.

---

## Dataset Description

The dataset includes product rating and review data with the following attributes:

- `author`: Reviewer name
- `country`: Country of origin
- `date`: Review date
- `domain`: Source website
- `extract`: Review text
- `language`: Language of the review
- `product`: Mobile phone name
- `score`: User-given rating
- `score_max`: Maximum possible rating
- `source`: Source of the rating

---

## Project Objective

Develop a recommendation system using:

- **Popularity-Based Filtering** – Recommend top-rated phones across users
- **Collaborative Filtering** – Recommend phones based on user similarity

---

## Methodology

### Data Processing

- Merged multiple CSV sources into a unified DataFrame
- Cleaned and preprocessed data:
  - Rounded scores to nearest integer
  - Handled missing values using median imputation
  - Encoded categorical variables (e.g., `lang`, `country`, `domain`)
  - Removed irrelevant or low-impact features (`phone_url`, `extract`)

### Recommendation Techniques

- **Popularity-Based Recommender**:
  - Aggregate and rank phones based on total score and number of ratings
  - Recommend top-N products with highest popularity

- **Collaborative Filtering (User-User)**:
  - Created a pivot table of users vs products
  - Used cosine similarity to identify similar users
  - Recommended phones based on neighbor preferences

---

## Key Observations

- `extract` and `phone_url` were non-contributory and excluded
- Most reviews were written in English
- Popular brands consistently appeared in top-ranked results
- Collaborative filtering provided more personalized suggestions

---

## Improvements achieved

Accuracy / Score
- Logistic Regression : 96%
- SVM model : 96%
- KNN Model : 97%
  
All the three models are close to 96-97% where as the KNN provides the higher value conpared to the three

Iterating the final model using varying hyperparameters yealds less significant improvement.

- The SVM model's C value was increased exponentially and found that 0.1 provided an 1% improvement but other higher values added very less improvement

Confusion Matrix
- The Type 1 error in Logistic Regression was 21 got reduced in SVM model to 19 and in KNN to 16
- The Tyep 2 error in Logistic Regression of 20 to 30 in SVM model and to 31 in KNN model
- The sum of True Postive and True Negatve remained alsomost equal across three models (1201 to 1204)

---

## Technologies Used

- **Python**
- **Pandas / NumPy** – Data manipulation
- **Matplotlib / Seaborn** – Visualization
- **Scikit-learn** – Cosine similarity and modeling

---

## Instructions

1. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

2. Run the notebook in Jupyter or JupyterLab.

3. Explore both recommendation strategies and compare the results.
