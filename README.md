# Cafe Sales Analysis

This project analyzes cafe transaction data from 2023 to understand sales performance, product sales, customer purchasing patterns, and revenue contribution.

The project was completed using Python in Jupyter Notebook and Tableau for data visualization.

## Project Overview

The analysis focuses on:

* Examining the overall sales performance.
* Identifying the best-selling products.
* Comparing product quantity and revenue.
* Analyzing monthly transaction and revenue trends.
* Exploring purchasing patterns based on payment method, order status, and spending level.
* Visualizing the results through Tableau dashboards.

## Dataset

The dataset contains cafe transaction records with the following columns:

* Transaction ID
* Item
* Quantity
* Price Per Unit
* Total Spent
* Payment Method
* Location
* Transaction Date

The original dataset contains around 10,000 records.

## Data Preparation

Before conducting the analysis, several data cleaning steps were performed:

* Checking missing values.
* Handling invalid values such as `ERROR` and `UNKNOWN`.
* Converting columns into the correct data types.
* Checking outliers using the IQR method.
* Removing duplicate records.
* Recalculating `Total Spent` based on quantity and price per unit.
* Creating additional columns for further analysis.

The additional columns include:

* Month
* Day Type
* Day Name
* Order Status
* Spending Level

The cleaned dataset contains approximately 7,562 valid transactions.

## Analysis

The project includes exploratory data analysis and statistical analysis using Python.

The analysis covers:

* Product sales performance.
* Revenue by item and product category.
* Monthly transaction trends.
* Monthly revenue trends.
* Payment method distribution.
* Weekday and weekend purchasing patterns.
* Relationship between product category, payment method, order status, and spending level.

Chi-Square Test of Independence and Cramér’s V were also used to examine the relationship between selected categorical variables.

## Data Visualization

The analysis results were presented through three Tableau dashboards:

### Overview Dashboard

Shows the general sales performance, including total sales, top-selling items, revenue by item, monthly transactions, and payment method distribution.

### Relationship Dashboard

Shows the relationship between product category, spending level, order status, payment method, and day type.

### Revenue Dashboard

Shows revenue contribution based on product category, purchase size, and spending level.

## Main Findings

Some of the main findings include:

* Coffee is the best-selling item based on quantity.
* The item with the highest quantity sold does not always generate the highest revenue.
* Sandwich and Smoothie generate higher revenue than Coffee even though their sales quantities are lower.
* Monthly transactions and revenue show different patterns throughout 2023.
* Spending level has a stronger relationship with product category compared to the other tested relationships.

## Tools Used

* Python
* Pandas
* Jupyter Notebook
* Tableau

## Project Files

* `Cafe_Sales_Data_Analysis_&_Visualization.ipynb` - Main analysis notebook.
* `cafe_sales_analysis.csv` - Dataset used for the analysis.
* `dirty_cafe_sales.csv` - Dataset before cleaning.
* `cleaned_cafe_sales.csv` - Dataset after cleaning.

## Project Limitation

This project focuses on descriptive and statistical analysis. The dataset is used to understand existing transaction patterns rather than building a predictive machine learning model.

The analysis is also limited to transaction data from 2023. Other factors such as customer demographics, promotions, weather, and operating costs are not included.
