# Milestone 1 – CIE: Data Transformation & Analysis

## Overview

This repository contains the individual assignment submission for **Milestone 1 – CIE**. The objective is to load, understand, clean, transform, analyze, and visualize the **Global Food Delivery Market** dataset using Python, Pandas, and Matplotlib.

The analysis explores food-delivery orders, order values, customer ratings, fulfillment time, cities, and cuisine categories.

## Repository Contents

- `global_food_delivery_enriched_market_2026.csv` – The food-delivery dataset used for the analysis.
- `Milestone_1 (1).ipynb` – The Jupyter Notebook containing the step-by-step Python code and analysis.
- `README.md` – Overview and instructions for this project.

## Steps Covered in the Notebook

1. **Importing Libraries:** Imported Pandas for data handling and Matplotlib for data visualization.

2. **Dataset Loading:** Loaded the CSV file using `pd.read_csv()`.

3. **Data Understanding:** Inspected the dataset using:
   - `.head()` to display the first five records.
   - `.shape` to find the number of rows and columns.
   - `.columns` to view column names.
   - `.info()` to inspect data types and non-null counts.
   - `.describe()` to view statistical summaries.

4. **Checking Missing Values:** Used `.isnull().sum()` to identify missing values in each column.

5. **Handling Missing Values:** Applied mean imputation to numeric columns using `fillna()` and `mean(numeric_only=True)`.

6. **Data Transformation:**
   - Converted `metro_city` to the category data type.
   - Converted `cuisine_category` to the category data type.
   - Converted `is_peak_hour` to Boolean.
   - Created a new column, `high_rating`, which is `True` when `customer_rating` is 4 or above.

7. **Insight Generation:** Generated the following information:
   - Total number of orders.
   - Average order value.
   - Average customer rating.
   - Average total fulfillment time.
   - City-wise total order value.
   - Cuisine-wise average order value.

8. **Data Visualization:** Created the following charts using Matplotlib:
   - City-wise Order Value (Bar Chart).
   - Cuisine-wise Average Order Value (Bar Chart).
   - Customer Rating Distribution (Histogram).

9. **Final Dataset Display:** Displayed the first ten records and the final dataset shape.

10. **Column Check and Removal:** Checked whether `cot_market_dynamics_rationale` exists in the DataFrame and removed it only if it is present.

## Dataset Information

- **Dataset file:** `global_food_delivery_enriched_market_2026.csv`
- **Number of records:** 8,000
- **Number of columns in the original CSV:** 26
- **Domain:** Global food delivery market
- **File format:** CSV

## Tools and Libraries Used

- Python
- Pandas
- Matplotlib
- Jupyter Notebook

## Conclusion

This project demonstrates the basic data-analysis process using Python. It includes reading a CSV dataset, understanding its structure, checking and handling missing numeric values, transforming columns, creating new information, generating insights, and presenting findings through charts.
