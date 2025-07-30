# Hands-on-Pandas-Assignment

# 📚 `tips` Dataset – Hands-on Pandas Assignment

This project is an assignment designed to practice fundamental Pandas operations using the popular `tips` dataset from the `seaborn` library. The goal is to practice essential data analysis steps, including data manipulation, filtering, grouping, and summarizing.

-----

### ✅ Step 0: Load Necessary Libraries and Prepare the Dataset

Before starting the analysis, import the `seaborn` and `pandas` libraries and load the `tips` dataset into a DataFrame.

```python
import seaborn as sns
import pandas as pd

# Load the 'tips' dataset
df = sns.load_dataset("tips")
```

-----

## 🚀 Assignment Steps

Complete the following steps sequentially to perform various analyses on the dataset.

### 📌 1. Basic Observations

Perform basic exploratory steps to get familiar with the dataset.

1.  Display the first 10 rows of the dataset.
2.  Print the number of rows and columns in the dataset.
3.  List all column names and their corresponding data types.
4.  Check which columns have missing data (null/NaN values).

-----

### 📌 2. Selection and Filtering

Practice selecting and filtering data that meets specific conditions.

5.  Filter and list the records where the `total_bill` is greater than 20.
6.  Select all customers who are both a `smoker` and have a `sex` of `Male`.
7.  Create a new DataFrame that contains only the `total_bill`, `tip`, and `day` columns.

-----

### 📌 3. Creating New Columns

Derive a new, meaningful column from the existing data.

10. Create a new column named `tip_rate`. This column should show the ratio of the tip to the total bill: `(tip / total_bill)`.

-----

### 📌 4. Grouping and Summarizing

Generate summary statistics by grouping the data into specific categories.

11. Group by the customers' `smoker` status and compare the average `tip` for each group.
12. Group by the `day` and `time` variables to find the average `total_bill` for each group.

-----

### 📌 5. Sorting and Value Counts

Analyze the distribution of categorical data.

13. Find the most frequently occurring day (the mode) in the `day` column.
14. Calculate the percentage (%) of female and male customers in the `sex` column.

-----

### 📌 6. Saving the Results

After all operations are complete, save your final, modified DataFrame to a CSV file.

15. Save the resulting DataFrame to your local directory with the name `tips_analysis.csv`.

<!-- end list -->

```python
# The index=False parameter prevents the DataFrame index from being written into the file.
df.to_csv("tips_analysis.csv", index=False)
```
