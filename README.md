# Shopping Dataset Analysis Using Pandas

## Project Overview

This project demonstrates the use of Python and the Pandas library for basic data exploration, cleaning, and preprocessing of a CSV dataset. The objective is to learn fundamental data analysis techniques such as handling missing values, filtering data, removing duplicates, creating derived columns, and exporting cleaned data.

## Objective

Learn Python basics and perform basic data exploration and cleaning using Pandas.

## Problem Statement

Perform the following tasks on a CSV dataset:

1. Load a CSV dataset into a Pandas DataFrame.
2. Explore the dataset using:
   - Head and tail records
   - Shape of the dataset
   - Column names
   - Data types
3. Handle missing values by:
   - Identifying null values
   - Filling or dropping missing data
4. Perform basic operations:
   - Filter rows
   - Select specific columns
5. Remove duplicate records.
6. Create a derived column:
   - `total_amount = price * quantity`
7. Save the cleaned dataset as a new CSV file.

## Technologies Used

- Python 3.x
- Pandas
- Jupyter Notebook

## Project Structure

```text
shopping-dataset-analysis/
│
├── data/
│   ├── shopping_dataset.csv
│   └── cleaned_shopping_dataset.csv
│
├── notebooks/
│   └── Shopping_Dataset_Analysis.ipynb
│
├── README.md
└── requirements.txt
```

## Steps Performed

### 1. Data Loading
- Imported the dataset into a Pandas DataFrame.

### 2. Data Exploration
- Viewed the first and last few records.
- Checked dataset dimensions.
- Inspected column names and data types.

### 3. Missing Value Handling
- Identified missing values using Pandas functions.
- Filled or removed missing entries where necessary.

### 4. Data Filtering and Selection
- Selected specific columns.
- Filtered records based on conditions.

### 5. Duplicate Removal
- Detected and removed duplicate rows.

### 6. Feature Engineering
- Created a new column:

```python
df["total_amount"] = df["price"] * df["quantity"]
```

### 7. Exporting Cleaned Data
- Saved the processed dataset as a new CSV file for further analysis.

## Output

The project generates:

- Jupyter Notebook (`.ipynb`)
- Cleaned CSV dataset
- Summary of preprocessing steps and findings

## Sample Code

```python
import pandas as pd

df = pd.read_csv("shopping_dataset.csv")

df["total_amount"] = df["price"] * df["quantity"]

df.to_csv("cleaned_shopping_dataset.csv", index=False)
```

## Conclusion

This project provides hands-on experience with Python and Pandas for data preprocessing. It covers essential data cleaning techniques that form the foundation of data analysis and machine learning workflows.
