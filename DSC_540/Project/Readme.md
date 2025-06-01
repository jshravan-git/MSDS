
# Data Preparation Project 

## Author
**Saravanan Janarthanan**

## Project Overview

This project demonstrates **Data Preparation** tasks. The objective is to demonstrate proficiency in collecting, cleansing, transforming, and visualizing data from multiple sources using Python and SQLite.

## Project Requirements

The project entails:

1. **Loading and transforming data from three formats:**
   - Flat file (e.g., CSV)
   - Web data via scraping
   - Web service using an API call

2. **Loading all cleaned/transformed data into SQLite as separate tables.**

3. **Merging the data from all sources into a single dataset using SQL joins.**

4. **Visualizing the cleaned and combined dataset with at least five visualizations.**

---

## Data Sources and Workflow

### 1. Flat File
- Load data from a flat file (e.g., CSV)
- Clean column headers (e.g., renaming "P/E" to "Price Earnings")
- Replace blanks and format header names for ease of querying
- Load the cleaned data into a SQLite table

### 2. Web Scraping
- Access and parse web page content
- Extract relevant data (e.g., tables or structured content)
- Clean and format the scraped data
- Load the data into a SQLite table

### 3. API Integration
- Use an API to request and receive structured data (e.g., JSON format)
- Parse and clean the response
- Load the resulting data into a SQLite table

---

## Merging and Visualization

- Join all three SQLite tables into a unified dataset using SQL
- Load the merged data into a pandas DataFrame
- Perform feature selection for visualization
- Create at least five meaningful visualizations using Python libraries

---

## Technologies Used

- **Python**: For scripting and data manipulation
- **SQLite**: To store and query intermediate data
- **Pandas**: For dataframes and merging
- **Matplotlib / Seaborn**: For data visualization
- **BeautifulSoup / Requests**: For web scraping
- **JSON / APIs**: For retrieving external data

---

## Usage

To reproduce the analysis:

1. Install required packages:
```bash
pip install pandas matplotlib seaborn requests beautifulsoup4 sqlite3
```

2. Run the Jupyter notebook in a local environment.
