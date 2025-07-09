# World Population Data Analysis with Pandas

## 📌 Project Overview

This project performs comprehensive data analysis and visualization on a global population dataset using **Python**, **Pandas**, **Seaborn**, and **Matplotlib**. It covers two major phases:

1. **Data Cleaning & Preparation**  
2. **Exploratory Data Analysis (EDA)**

The dataset, sourced from Kaggle, has been slightly modified to add diversity and simulate real-world imperfections (e.g., missing values).

## ⚙️ Libraries Required

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```


---

## 🧰 Tools Used

- Python 3
- pandas
- Jupyter Notebook / Google Colab

---

## 🚀 Cleaning Process

### 1. ✅ Steps Performed:
- Missing Value Detection:
  Used df.isnull().sum() to count nulls across all columns.

- Duplicate Removal:
  Detected using df.duplicated().sum() and removed with df.drop_duplicates(inplace=True).

- Data Type Inspection:
  Used df.dtypes and df.select_dtypes() to classify numeric and non-numeric columns.

### 2. Column Renaming & Formatting:
 - Renamed verbose columns for clarity.

 - Set display format

### 3.String Normalization
 - Cleaned and standardized country and continent names using .str.strip(), .str.upper(), etc.


## 🔍 Exploratory Data Analysis (EDA)

### 🧪Correlation Matrix 
- Identified strong positive correlations between population columns across years.

- Found weak correlations between population and area, density, or growth rate.

### 🌍Grouping By Continent 
- Found Asia had the highest average population and density.

- Discovered Oceania had the smallest numbers and included mostly small island nations.

### 📉Population Growth by Continent(1970-2022)
- Transposed grouped data for better visualization
- Observed:

   - Rapid growth in Asia, especially post-2000.
   - Oceania showed minimal change.
   - Other continents grew steadily.

### 📦Boxplots to Identify Outliers
- Clearly displayed outliers in the population columns.

- Noted these are expected due to large variation in country sizes.

## 📊 Key Insights
- Population trends are highly correlated over time, showing consistent growth patterns.
- Asia leads in both average population and density, while Oceania is lowest.
- Boxplots reveal extreme outliers, expected due to vast country size differences.
- Grouping and transposing data helped visualize growth trends per continent over five decades.


